# oauth-test

Sample implementation of GitHub OAuth App working with Cloudflare Workers + KV.

- Article: [Cloudflare Workers + KV で OAuth2.0 クライアント](https://zenn.dev/inaniwaudon/articles/7fa50a744cb67a)

## Development

Edit `wrangler.toml` and `.dev.vars` as follows.

```bash
GITHUB_CLIENT_SECRET=<github_client_secret>
```

Run the following commands.

```bash
yarn
yarn run dev
```

### Deployment

```bash
wrangler secret put GITHUB_CLIENT_SECRET --env production
wrangler deploy
```

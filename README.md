# Salong Ilinium

Self-hosted website and CMS for Salong Ilinium. 

## Commands

```sh
npm install
npm test
npm run build:strato
```

The current salon content is stored in `public/api/seed.json` and imported by the one-time installer. 

## Security

- Database credentials exist only in ignored `api/config.php`.
- Passwords use PHP's `password_hash` and are never stored as plaintext in MySQL.
- Admin sessions use HTTP-only, Secure, SameSite cookies.
- Database operations use prepared statements and strict table/column allowlists.
- Uploaded files are MIME-validated and script execution is blocked in `uploads/`.

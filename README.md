# Htaccess WordPress

An Apache [`.htaccess`](.htaccess) reference for WordPress, with examples for browser caching, compression, MIME types, and access rules.

## ✨ What's included

- Cache-Control and expiration rules for static assets, including images and fonts.
- Gzip and optional Brotli compression, subject to enabled Apache modules.
- MIME-type mappings for fonts and other assets.
- Header examples for proxy caching and ETags, plus a Keep-Alive example that depends on server configuration.
- WordPress rewrite rules and restrictions for selected files and directories.

## 🛠️ Apply selected rules

1. Back up your current `.htaccess` and review the reference file against your host's Apache version, enabled modules, and override settings.
2. Apply only the compatible rules to your existing file on a staging site. Preserve your site's WordPress rewrite block and any hosting- or plugin-managed rules.
3. Test the homepage, permalinks, admin access, and static assets before deploying. Restore the backup if Apache reports a configuration error.

> [!IMPORTANT]
> Keep your existing `.htaccess`. A [`<DirectoryMatch>` block](https://httpd.apache.org/docs/2.4/mod/core.html#directorymatch) belongs in Apache server or virtual host configuration. Skip that block when editing `.htaccess`.

## 🤝 Contributing

Use [issues](https://github.com/informigados/htaccess-wordpress/issues) or pull requests to suggest changes. Include the Apache version and hosting context when reporting a compatibility problem.

## 👥 Authors

- [Alex Brito](https://github.com/alexbritodev)
- [INformigados](https://github.com/informigados)

## 📄 License

This project is licensed under the [MIT License](LICENSE).

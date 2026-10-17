# Security and Privacy

## Do not commit sensitive information

Before pushing this project to a public GitHub repository, make sure the repository does not contain:

- Private/internal IP addresses
- Internal company URLs
- Private Google Drive or Google Sheets links
- Passwords
- API keys
- Access tokens
- Cookies or session data
- Confidential documents
- Personal JSON backups containing private links

## Personal backup files

Keep your exported `my-workspace-backup.json` outside the public repository when it contains private or work-related links.

## Browser storage

The dashboard uses browser local storage for its working data. Data stored in one origin is not automatically available on another origin or another device.

## Reporting an issue

If you discover a security issue in a customized deployment, remove sensitive information from public commits immediately and rotate any credentials that may have been exposed.

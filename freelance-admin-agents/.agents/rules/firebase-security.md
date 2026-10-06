# Firebase Security

Firebase is shared between PUBLIC_SITE and ADMIN_SITE.

Public website:
- Read public/published content.

Admin:
- Authenticated administrators can create, read, update, delete, and publish content.

Never trust:
- client role fields
- localStorage role
- hidden UI buttons
- URL parameters

Authorization must be enforced by Firebase/security rules and trusted server-side logic where applicable.

Never expose service-account credentials or privileged secrets to the browser.

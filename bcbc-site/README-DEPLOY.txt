BCBC MASTER PACKAGE V2

Purpose:
- Static website package for Baxter/Apache or GitHub Pages-style hosting.
- Includes main site, Technician Tools page, founder page, projects page, public resume, private resume, and SVG graphics.

Recommended Baxter deploy:
1. Unzip this package.
2. Backup current web root first:
   sudo mkdir -p /var/www/html-backups
   sudo cp -a /var/www/html /var/www/html-backups/html-$(date +%Y%m%d-%H%M%S)
3. Deploy:
   sudo rsync -a --delete bcbc_master_package_v2/ /var/www/html/
4. Fix ownership if needed:
   sudo chown -R www-data:www-data /var/www/html

Name guidance:
- Public-facing founder name: William James Franza.
- Formal/legal/adopted name for required records: William A. James.
- Keep private resume private; publish public resume.

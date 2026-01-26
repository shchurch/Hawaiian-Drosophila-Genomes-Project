# GitHub Pages Deployment Guide

## Enabling GitHub Pages

To deploy this website to GitHub Pages, follow these steps:

1. **Go to Repository Settings**
   - Navigate to your repository on GitHub
   - Click on "Settings" tab

2. **Enable GitHub Pages**
   - In the left sidebar, click on "Pages"
   - Under "Source", select the branch you want to deploy (e.g., `main` or `copilot/create-static-website-for-project`)
   - Keep the folder as `/ (root)`
   - Click "Save"

3. **Wait for Deployment**
   - GitHub will automatically build and deploy your site
   - This usually takes 1-2 minutes
   - You'll see a green checkmark when it's ready

4. **Visit Your Site**
   - Your site will be available at: `https://shchurch.github.io/Hawaiian-Drosophila-Genomes-Project/`
   - The URL is shown at the top of the Pages settings

## Custom Domain (Optional)

If you want to use a custom domain:

1. Add a `CNAME` file to the repository root with your domain name
2. Configure DNS settings with your domain provider
3. Add the custom domain in GitHub Pages settings

## Updating the Site

To update the website:

1. Make changes to the files locally or via GitHub web interface
2. Commit and push changes
3. GitHub Pages will automatically rebuild and deploy (takes 1-2 minutes)

## Troubleshooting

**Build Failures:**
- Check the Actions tab for build logs
- Ensure `_config.yml` is valid YAML
- Verify all required files are committed

**404 Errors:**
- Make sure GitHub Pages is enabled
- Check that the branch and folder settings are correct
- Verify the baseurl in `_config.yml` matches your repository name

**CSS Not Loading:**
- Ensure `baseurl` in `_config.yml` is set correctly
- Check that CSS files are in the `assets/css/` directory
- Clear browser cache and try again

## Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Minima Theme](https://github.com/jekyll/minima)

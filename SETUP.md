# Quick Setup Guide

## Deploy to GitHub Pages (Easiest Method)

1. **Create/Update your GitHub repository**
   - Go to github.com and create a new repo named `vineetjnair9.github.io`
   - Or use your existing repository

2. **Upload these files**
   - You can drag and drop all files from this folder to GitHub
   - Or use git commands:
     ```bash
     git init
     git add .
     git commit -m "New Jekyll Minima site"
     git branch -M main
     git remote add origin https://github.com/vineetjnair9/vineetjnair9.github.io.git
     git push -u origin main
     ```

3. **Enable GitHub Pages**
   - Go to your repository Settings
   - Click "Pages" in the left sidebar
   - Under "Source", select "Deploy from a branch"
   - Choose `main` branch and `/ (root)` folder
   - Click Save

4. **Wait a few minutes**
   - GitHub will build your site automatically
   - Visit `https://vineetjnair9.github.io` to see it live

## Customize Your Site

### Edit Content
- **Homepage**: Edit `index.md`
- **About page**: Edit `about.md`
- **Publications**: Edit `publications.md` - just add your papers in markdown
- **CV**: Edit `cv.md`

### Add Publications (Easy!)
Just edit `publications.md` and add entries like:

```markdown
**Your Paper Title Here**  
Authors: Smith, J., **Vineet J Nair**, Jones, A.  
*Journal Name*, Vol 10, pp. 123-145, 2024  
[Paper](https://link-to-paper.com) | [Code](https://github.com/yourrepo)
```

No CSV files needed!

### Add Blog Posts (Optional)
Create files in `_posts/` folder with name: `YYYY-MM-DD-title.md`

### Change Theme Colors
Edit `_config.yml` and change the `skin` value:
- `classic` (default, blue)
- `dark` (dark mode)
- `auto` (follows system preference)
- `solarized-light` or `solarized-dark`

### Add Your Photo
1. Create folder: `assets/images/`
2. Add your photo: `assets/images/profile.jpg`
3. Add to any page: `![Your Name](/assets/images/profile.jpg)`

## Test Locally (Optional)

If you want to preview before deploying:

1. Install Ruby (https://www.ruby-lang.org/en/downloads/)
2. Install Bundler: `gem install bundler`
3. In this folder, run:
   ```bash
   bundle install
   bundle exec jekyll serve
   ```
4. Open http://localhost:4000

## Troubleshooting

**Site not showing up?**
- Check Settings > Pages shows "Your site is published at..."
- Wait 5-10 minutes after first push
- Make sure files are in the root of the repository

**Want to use a different URL?**
- Change `url:` in `_config.yml`
- Change `baseurl:` if using a project site (not username.github.io)

## Need Help?

- Jekyll docs: https://jekyllrb.com/docs/
- Minima theme: https://github.com/jekyll/minima
- GitHub Pages: https://docs.github.com/en/pages

# GS004 Google Review Helper

Grand Senheng Sri Dagangan Kuantan. Ready for GitHub Pages, with no installation or build required.

## Publish the webpage publicly

1. Extract this ZIP on your computer. Upload the extracted files, not the ZIP itself.
2. Sign in to GitHub and create a new repository called `gs004-review-helper`.
3. Set the repository visibility to **Public**. You can enable **Add README** when creating it.
4. Inside the repository, choose **Add file > Upload files**. Upload `index.html` and `gs004-review-comments.json` directly to the repository's top level. The included README and `.nojekyll` can be uploaded too. Do not place the website files inside an extra folder.
5. Click **Commit changes** and save to the `main` branch.
6. Open **Settings > Pages**.
7. Under **Build and deployment**, choose **Deploy from a branch**.
8. Select **main** and **/(root)**, then click **Save**.
9. Wait for deployment to finish, then use **Visit site** in the Pages settings. GitHub says publication can take up to 10 minutes.

Your address will normally be:
`https://YOUR-GITHUB-USERNAME.github.io/gs004-review-helper/`

Use the website URL, not the repository URL, when sharing with customers. After GitHub Pages publishes successfully, customers can open it without a GitHub or ChatGPT login. They use their own Google account to submit the Google review.

Official instructions:
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Included files

- `index.html`: complete webpage, styling, JavaScript and embedded backup comments.
- `gs004-review-comments.json`: 350 editable suggestions across seven categories.
- `.nojekyll`: tells GitHub Pages to serve the static files without Jekyll processing.
- `README.md`: these instructions.

## How it works

Enter a staff code, choose a category, fill in details, then choose and edit a review. Copy the result and paste it on Google's review page. Customers choose their own rating and submit manually.

The earning calculation uses the supplied 5% maintenance deduction. For example, RM1,000 at 50% cashback gives RM475 in S-Coin value, or 47,500 S-Coin. Redemption input is the RM value used.

The Google destination retains the Place ID supplied in the original GS004 file: `ChIJV_UaAZG6yDERBfK-vHdQRu8`. Confirm the correct outlet appears before distributing the link.

No API keys, server or paid services are needed. The HTML contains backup comments if the JSON cannot load. Staff and form details are kept in this browser session; suggestion history is kept in this browser only. No customer information is sent to a database by this helper.

## Editing comments later

Keep the JSON filename, version `8`, category names and placeholder names unchanged. The current loader expects 50 comments in each of the seven categories. After editing JSON, also update the matching `fallbackData` block in `index.html` if you want the embedded backup to match. Customer edits on the page apply to that review only and do not change the templates.

For staff-specific links, append `?staff=SH12345` to your website URL, replacing the example with the real staff code.

This ZIP is ready to publish; downloading it alone does not create a live GitHub Pages site.

## Warranty comment update — 21 September 2026

The five service/warranty categories each have 50 rewritten comments in casual Malaysian Malay. S-Coin earning and redemption comments remain unchanged.

- **RW when buying:** eligible small appliances with paid RW have an extra year, for 2 years in total. Comments describe replacement with a new unit 1-to-1 on the spot if the item breaks during coverage, based on its original purchase value.
- **RW claims:** comments say the item broke and the customer received that new-unit replacement. The previous separate replacement-outcome choices were removed because 1-to-1 and original-price value describe the same benefit.
- **PlusOne® when buying:** members receive a free additional year for selected eligible products after the manufacturer warranty. One manufacturer year becomes two total; two manufacturer years become three.
- **PlusOne® claims:** comments describe an item breaking after the manufacturer warranty expired, with the free additional member year still active and a covered repair saving the customer money.
- **Service:** longer comments cover help carrying items, promotions, suitable product suggestions, friendliness, demonstrations and payment choices. Customers should select and edit only wording that matches their actual experience.

Warranty scenarios follow the outlet details supplied for this update. They are not an independent audit of all Senheng terms.

To update an existing GitHub Pages site, replace both `index.html` and `gs004-review-comments.json` with the files from this ZIP and commit to the publishing branch. The embedded backup comments have also been updated.

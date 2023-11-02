# Local Gov Static

This theme is built using Jekyll and Tailwind CSS and is designed as a starter template for Local Government microsites.

It has been setup to follow the process in [this blog post](https://mzrn.sh/2022/04/09/starting-a-blank-jekyll-site-with-tailwind-css-in-2022/) so it uses post-css to process the styles and jekyll to build the pages.

## Usage

- Fork this repository
- Install the npm dependencies for tailwind using `npm install`
- Install the gem dependencies using `bundle install`
- Run the site locally using `bundle exec jekyll serve`

## Customising the theme

As this app uses Tailwind CSS for styling you can customise the `tailwind.config.js` as per any other tailwind site.

The only custom settings are for the action colour which can be customised as needed. There is a light (200), regular (500) and dark (900) setting for the action that is used in various places throughout the site.

```js
colors: {
    action: {
        200: "#E9EEF3'",
        500: "#385889",
        900: "#0E335B",
    },
},
```

## HTML Proofing

To proof the HTML and check for broken links, run:

```bash
bundle exec jekyll build
bundle exec htmlproofer ./_site
```

## Hosting with S3 and Cloudfront

How you host your static site is up to you, but there are some example files that can be used to get you started with hosting in AWS with S3 and cloudfront.

**The files are provided as a starting point, so ensure you understand what they do and that they are suitable for your needs before using!**

Use the `s3-cloudfront.yml` file to create a new stack in cloudfront using either AWS CLI or the [AWS console](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/cfn-console-create-stack.html). This will create a bucket and a cloudfront distribution for you.

### Manually deploying to S3

You can manually build and deploy the site from your local machine using the following commands, replacing bucket-name with the name of your bucket and my-profile with the name of your aws profile:

```bash
JEKYLL_ENV=production bundle exec jekyll build
aws s3 sync _site s3://bucket-name --delete --cache-control max-age=300 --profile my-profile
```

### Deploying using GitHub Actions

There is an example GitHub workflow configured to deploy the changes to the S3 bucket when you push to the main branch, and then invalidate the Cloudfront cache.

Rename `.github/workflows/s3-deploy.yml.example` to `.github/workflows/s3-deploy.yml`.

Configure an OpenID Connect (OIDC) role [following this tutorial](https://aws.amazon.com/blogs/security/use-iam-roles-to-connect-github-actions-to-actions-in-aws/).

Then, configure the following GitHub Actions secrets in your GitHub repo:

- ‌AWS_ROLE_NAME
- AWS_BUCKET_NAME
- CLOUDFRONT_DISTRIBUTION_ID

It will run the GitHub Action automatically when ever changes are pushed to the `main` branch.

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/FutureNorthants/LocalGovStatic. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](https://www.contributor-covenant.org/) code of conduct.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

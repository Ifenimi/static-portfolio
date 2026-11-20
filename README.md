# Adedamola Oluwanisola — DevOps Portfolio

[GitHub](https://github.com/Ifenimi) · [LinkedIn](https://www.linkedin.com/in/adedamola-oluwanisola-60337714b/)

My portfolio of hands-on work across AWS infrastructure, Bash automation, and application development. My DevOps goal is to bridge development and operations through predictable infrastructure, automated workflows, and faster feedback.

The site is designed for Amazon S3 static website hosting. It uses plain HTML, CSS, and JavaScript; no build step or server-side runtime is required.

## Featured projects

- [AWS Three-Tier VPC](https://github.com/Ifenimi/aws-three-tier-vpc) — public and private subnets, NAT Gateway, security groups, and connectivity validation.
- [Bash Automation Exercises](https://github.com/Ifenimi/bash_scripting_exercises) — five shell utilities emphasizing validation, safe path handling, and modular scripts.
- [Skyline Weather](https://github.com/Ifenimi/weather_application_2026) — responsive weather application with a Node.js/Express API.
- [S3 Static Portfolio](https://github.com/Ifenimi/static-portfolio) — this static site and its S3 hosting setup.

## Files

- `index.html` — portfolio home page
- `index.css` — responsive styles
- `index.js` — mobile navigation and current-year footer
- `error.html` — custom not-found page for S3
- Image files in the repository root — portrait and project screenshots used by the site

## Run locally

Open `index.html` in a browser, or serve the repository root with any static file server. Keep the image files alongside the HTML files so their relative paths resolve.

## Host on Amazon S3

1. Create an S3 bucket for the website and upload the HTML, CSS, JavaScript, and image files to the bucket root.
2. In the bucket's **Properties**, enable **Static website hosting**.
3. Set the index document to `index.html` and the error document to `error.html`.
4. Configure the bucket's access policy for public website reads if serving directly from the S3 website endpoint. Review the bucket's Block Public Access settings before enabling public access.
5. Open the **Bucket website endpoint** shown in the static website hosting settings.

S3 website endpoints serve HTTP. For HTTPS and a custom domain, put Amazon CloudFront in front of the bucket and configure the domain and certificate there.

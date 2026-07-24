# JobLens AI

JobLens AI is a Chrome extension that checks a job description against your CV and gives you a quick match view. You upload your CV once, then it shows your match score, strengths, skill gaps, and a few practical suggestions while you are browsing job pages.

It currently works on LinkedIn, Indeed, and Reed. The extension reads the job page content and sends it for analysis, so you do not need to copy and paste the whole description every time.

## What you need

- A Chrome browser
- An NVIDIA API key from [build.nvidia.com/settings/api-keys](https://build.nvidia.com/settings/api-keys)
- Your CV in a file you can upload

The extension uses NVIDIA's free model, so you do not need to pay for usage just to try it.

## How to load the extension

1. Download or clone this project.
2. Open Chrome and go to the extensions page.
3. Turn on Developer mode.
4. Click Load unpacked.
5. Select the `chrome-mv3-dev` folder if you want the development build, or `chrome-mv3` if you want the production build.

## How to use it

1. Open the extension popup.
2. Paste your NVIDIA API key.
3. Upload your CV.
4. Open a job page on LinkedIn, Indeed, or Reed.
5. Click the Start button on the extension home page.

After that, JobLens will scan the job page and show you the analysis.

## Tech stack

- NVIDIA Llama 3.1 8B Instruct free model
- React
- Vite
- WXT
- Tailwind CSS

## Notes

- This extension currently works on LinkedIn, Indeed, and Reed only.
- If the job page is not on one of those sites, the scan will not work properly.
- For development, the `chrome-mv3-dev` folder is the safer one to load because it includes the dev setup.

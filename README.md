This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
# Captions-Generator
Here’s a detailed README you can use for your **Captions Generator** app on GitHub:

---

# Captions Generator

Captions Generator is a web-based application that allows users to upload videos and automatically generate captions using AWS Transcribe. The generated captions are then synced and embedded into the video at the appropriate timestamps using FFmpeg. This application is built using modern web technologies like Next.js, Tailwind CSS, AWS services, and FFmpeg for video processing.

## Features

- **Video Upload**: Users can upload videos directly through the app.
- **Automatic Caption Generation**: Uses AWS Transcribe to automatically generate captions from the audio in the video.
- **Caption Syncing**: Captions are accurately synced with the video using FFmpeg to ensure they appear at the right times.
- **Downloadable Video with Captions**: Once the captions are generated and embedded, users can download the video with captions directly from the app.

## Tech Stack

- **Frontend**: [Next.js](https://nextjs.org/), [Tailwind CSS](https://tailwindcss.com/)
- **Backend**: AWS S3, AWS Transcribe, [FFmpeg](https://ffmpeg.org/)
- **Hosting**: Deployed on platforms like Netlify/Vercel (depending on your deployment preference).

## How It Works

1. **Upload Video**: The user uploads a video file through the web interface.
2. **Storage on AWS S3**: The uploaded video is stored in an AWS S3 bucket for processing.
3. **AWS Transcribe**: AWS Transcribe processes the audio track of the video and generates a transcript (captions) with timestamps.
4. **Caption Embedding with FFmpeg**: The generated captions are then synced and embedded into the video using FFmpeg, creating a final video file with captions.
5. **Downloadable Video**: The user can download the video with embedded captions.

## Prerequisites

To run this app locally or on your server, ensure you have the following set up:

1. **AWS Account**: 
   - You need to create an AWS account and configure AWS credentials for your app.
   - Set up an S3 bucket and enable AWS Transcribe in your account.
   
2. **FFmpeg Installation**: 
   - Install FFmpeg on your machine. You can download it from the official [FFmpeg website](https://ffmpeg.org/download.html).
   
3. **Next.js**: 
   - Make sure you have Next.js installed to run the frontend.

## Installation

### Clone the Repository

```bash
git clone https://github.com/Nishchay412/captions-generator.git
cd captions-generator
```

### Install Dependencies

```bash
npm install
```

### AWS Configuration

Ensure that you have your AWS credentials set up and configured correctly for S3 and Transcribe.

- Set up environment variables for your AWS credentials:

```
AWS_ACCESS_KEY_ID=<your-access-key-id>
AWS_SECRET_ACCESS_KEY=<your-secret-access-key>
S3_BUCKET_NAME=<your-s3-bucket-name>
```

### Run Locally

Start the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

## Deployment

The app can be deployed to platforms like [Netlify](https://www.netlify.com/) or [Vercel](https://vercel.com/). Make sure to include your environment variables in the deployment settings to allow access to AWS services.

### Steps for Deployment on Vercel:

1. Push your project to a GitHub repository.
2. Link your repository to Vercel.
3. Set up the environment variables in the Vercel dashboard.
4. Deploy your app!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [AWS](https://aws.amazon.com/) for the Transcribe service.
- [FFmpeg](https://ffmpeg.org/) for video processing.
- [Next.js](https://nextjs.org/) and [Tailwind CSS](https://tailwindcss.com/) for building the frontend.

---

Feel free to update any specific details regarding your deployment or add additional sections if necessary!

![captions diagram](https://github.com/user-attachments/assets/3e207ae8-1426-4422-a44d-6ecbe4eb8a9f)



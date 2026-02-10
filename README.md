<p align="center">
  <a href="https://bagisto.com/en/headless-commerce/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/bagisto/temp-media/0b0984778fae92633f57e625c5494ead1fe320c3/dark-logo-P5H7MBtx.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://bagisto.com/wp-content/themes/bagisto/images/logo.png">
      <img src="https://bagisto.com/wp-content/themes/bagisto/images/logo.png" alt="Bagisto logo">
    </picture>
  </a>
</p>

<p align="center">
    <a href="https://bagisto.com/en/headless-commerce/">Website</a> | <a href="https://headless-doc.bagisto.com/bagisto-native/integration-guide/getting-started">Documentation</a> | <a href="https://forums.bagisto.com/">Forums</a> | <a href="https://www.facebook.com/groups/bagisto/">Community</a>
</p>

<p align="center">
    <a href="https://twitter.com/intent/follow?screen_name=bagistoshop"><img src="https://img.shields.io/twitter/follow/bagistoshop?style=social"></a>
    <a href="https://www.youtube.com/channel/UCbrfqnhyiDv-bb9QuZtonYQ"><img src="https://img.shields.io/youtube/channel/subscribers/UCbrfqnhyiDv-bb9QuZtonYQ?style=social"></a>
</p>

<p align="center">
    <a href="https://packagist.org/packages/bagisto/bagisto"><img src="https://poser.pugx.org/bagisto/bagisto/license.svg" alt="License"></a>
</p>

# Bagisto Native Commerce

**Bagisto Native Commerce** is a ready-to-use storefront built on Bagisto Headless with Bagisto Native integration, enabling any React or Next.js application to seamlessly work with native mobile apps, modern frontend frameworks, and API-driven architectures.

You can directly use this storefront without building everything from scratch.

---

##  What We Focus On
- **Native-first** commerce experiences
- **Modern frontend stacks** (Next.js, React)
- **Mobile bridges** & integrations
- **Reusable SDKs** & utilities

## Packages
| Package | Description |
|---------|-------------|
| `@bagisto-native/react` | React wrappers for the Web Components included in your projects |
| `@bagisto-native/core` | Core utilities and shared logic |



## Prerequisites
Before starting, ensure you have:
- **Node.js 18** or higher
- **React/Next.js** project 
- **Bagisto store**
- **pnpm** installed

---

## Step 1: Project Setup

### 1. Clone/Create the Storefront
If you haven't already, you can create a new storefront or use this repository directly:
```bash
git clone https://github.com/bagisto/bagisto-native-commerce
cd bagisto-native-commerce
```

### 2. Install Dependencies
```bash
pnpm install
```

### 3. Configure Environment
Create a `.env.local` file and add your Bagisto API details. This keeps your settings secure and organized.

### One-Click Deploy to Netlify

Click the button above to deploy your own copy of Bagisto Native Commerce to Netlify instantly!


[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/bagisto/bagisto-native-commerce)

- *Note:* Add env variables in Netlify dashboard

---

## Step 3: Connect Native Apps

Once your Next.js project is running (e.g., at `http://localhost:3000`), you can connect it to the native mobile applications.

### iOS: Set Up for iOS App
1. **Clone the iOS Repository:**
   ```bash
   git clone https://github.com/SocialMobikul/BagistoNative_iOS.git
   cd BagistoNative_iOS
   ```
2. **Open in Xcode:**
   ```bash
   open BagistoNative.xcodeproj
   ```
3. **Configure Base URL:**
   Find the `base_url` variable in your Swift code and replace it with your project URL:
   ```swift
   let base_url = "http://localhost:3000"
   ```
4. **Build & Run:** Select a simulator and click **Run**.

### Android: Set Up for Android App
1. **Clone the Android Repository:**
   ```bash
   git clone https://github.com/SocialMobikul/BagistoNative_android.git
   cd BagistoNative_android
   ```
2. **Open in Android Studio:** Open the project folder.
3. **Configure Base URL:**
   Find the `base_url` variable in `Constants.java` (or equivalent):
   ```java
   public static String base_url = "http://localhost:3000";
   ```
4. **Build & Run:** Select an emulator and click **Run**.

---

## Helpful Resources
- [Bagisto Native iOS](https://github.com/SocialMobikul/BagistoNative_iOS)
- [Bagisto Native Android](https://github.com/SocialMobikul/BagistoNative_android)
- [Official Documentation](https://headless-doc.bagisto.com/bagisto-native/integration-guide/getting-started)

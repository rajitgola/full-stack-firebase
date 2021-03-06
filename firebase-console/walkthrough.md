# Walkthrough

We'll kick this party off with a quick run down of the Firebase Console.

It's how you'll interact with many of the Firebase features.

You'll need your Dashboard to configure your services and watch data flow through your project. Most of the Dashboard's functions are also accessible via the Firebase Tools command-line interface.

Command-line interface is a mouthful, so we'll refer to it as a CLI.

## firebase.google.com

So let's log in to Firebase. Visit [firebase.google.com](https://firebase.google.com/) and click the SIGN IN button

You'll sign in with your Google account and then land on your project selection screen.

Click "Add project" or select a project that you've already created.

![Add A Project](https://goo.gl/HjLmzL)

Once your project is live you'll be taken to that project's overview.

The project overview has one button that we use, "Add Firebase to your web app".

You can copy/paste values from this popup directly into your 'index dot html'.

![Add Firebase to your web app](https://goo.gl/LCK1fW)

Now notice the gears button. We won't spend much time here, but it's good to click around. Notice that you can change your project name and generate service accounts. We'll use the service accounts later when we're using Node.js in admin mode.

But let's continue on to the left bar.

![Project Overview](https://goo.gl/wMS5Qq)

The left bar has four sections, Develop, Stability, Analytics and Grow. The first section, Develop, is the one that we use for web. The other sections are mobile only.

Google rolled a bunch of their mobile platform products into the Firebase brand; however, Google's web products, such as Analytics and AdSense, are not under the Firebase brand

So let's start with Authentication.

## Firebase Authentication

Our user accounts list is empty, because we haven't enabled any sign-in methods, so let's do that. We have a variety of sign-in methods.

![Sign-In Methods](https://goo.gl/4GFwXV)

Our favorites are Email/Password and Google. So let's enable those methods. Next we'll need to make sure that our domains are authorized, especially for development.

Later in the course we'll be coding on Glitch.com. So let's authorize the Glitch.me domain. Glitch serves its pages up on Glitch.me, not on Glitch.com.

![Authorized Domains](https://goo.gl/K4o6Wn)

Let's also allow creation of multiple accounts per email address. This will automatically merge duplicate accounts created under the same email address. It's common for users to create an email/password account with a GMail address and later try to log in with Google using that same GMail address.

Now let's click through the Templates and Usage tabs.

![Authentication Templates](https://goo.gl/cqbxgr)

Firebase will send some email on your behalf, so it's nice to customize those emails.

And you'll have to pay for phone authentication if your app gets enormous. Having a hugely successful app would be a great problem to have. We hope to someday suffer that plight and spend more time monitoring usage.

But until then... let's forge ahead to Firebase's juicy core, the databases.

The Database section will give you two options, the Realtime Database or Cloud Firestore. The Realtime Database has tabs for Data, Rules, Backups and Usage. We can use the Data tab to view and modify the data in our JSON tree.

![Realtime Database Data](https://goo.gl/sPVPcK)

The Rules tab is great for visualizing and testing security rules. You can use the security rules simulator to simulate reads and writes. This is useful for making sure that your data is locked down and secure.

Moving on... the Backups tab is great once you're in production. You'll want to enable frequent database backups. They're cheap insurance against data loss.

And the Usage tab will, as we've seen before, help you manage your costs as you scale.

Let's continue on to the Storage section.

## Firebase Storage

![Firebase Storage](https://goo.gl/vzTRMG)

It's pretty spare with only two tabs, Files and Rules. We can use the File browser to create folders and upload files. Once we have files in our Storage bucket we can also view file details and some metadata. We'll cover security rules for Storage in a later chapter.

So let's continue on to Hosting!

![Firebase Hosting](https://goo.gl/Jy9jDp)

You'll mostly use Hosting's Dashboard tab to connect a custom domain. Firebase Hosting provides a \*.firebaseapp.com subdomain for each project. But when you're ready for real users, you'll want a custom domain with free SSL certs. You can also manage your deploys and review your deployment history.

The Usage tab is, again, most useful for cost control if your site gets popular.

So on to Functions.

## Firebase Functions

![Firebase Functions](https://goo.gl/SW1R2d)

Cloud Functions for Firebase is the "serverless" glue that holds your apps together. There's nothing to see here now, but we'll get very familiar with both the Dashboard and Logs tabs.

Cloud Functions are deployed via Firebase's CLI. We'll use the terminal to deploy our Functions, but we'll monitor the deploys here. We'll also spend time on the Logs and Usage tabs to make sure our Functions behave themselves.

And finally, let's click the Modify pricing plans button to see our options.

## Pricing

![Firebase Pricing](https://goo.gl/M1sroi)

Blaze includes the same free usage as Spark, but you'll pay as you exceed those limits.

All of our development usage and some of our production usage falls within the free limits.

Flame is never cheaper than Blaze... it's just price capped at 25 US dollars

We use Blaze for all of our projects.

## Conclusion

And that's the Firebase Console!

We'll dive deeper into each console section as we learn the associated Firebase features.

There's a lot to learn here, but you'll need a rich, active project for it to get interesting


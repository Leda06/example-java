[![example-java](https://github.com/koyeb/example-java/actions/workflows/deploy.yaml/badge.svg)](https://github.com/koyeb/example-java/actions)

<div align="center">
  <a href="https://koyeb.com">
    <img src="https://www.koyeb.com/static/images/icons/koyeb.svg" alt="Logo" width="80" height="80">
  </a>
  <h3 align="center">Koyeb Serverless Platform</h3>
  <p align="center">
    Deploy a Java application on Koyeb
    <br />
    <a href="https://koyeb.com">Learn more about Koyeb</a>
    ·
    <a href="https://koyeb.com/docs">Explore the documentation</a>
    ·
    <a href="https://koyeb.com/tutorials">Discover our tutorials</a>
  </p>
</div>


## About Koyeb and the Java example application

Koyeb is a developer-friendly serverless platform to deploy apps globally. No-ops, servers, or infrastructure management.  This repository contains a Java application you can deploy on the Koyeb serverless platform for testing.

This example application is designed to show how a Java application can be deployed on Koyeb.  You can follow the associated [deploy guide](https://koyeb.com/docs/deploy/java) to learn more about the application and how to extend it.

## Getting Started

Follow the steps below to deploy and run the Java application on your Koyeb account.

### Requirements

You need a Koyeb account to successfully deploy and run this application. If you don't already have an account, you can sign-up for free [here](https://app.koyeb.com/auth/signup).

### Deploy using the Koyeb button

The fastest way to deploy the Java application is to click the **Deploy to Koyeb** button below.

[![Deploy to Koyeb](https://www.koyeb.com/static/images/deploy/button.svg)](https://app.koyeb.com/deploy?name=example-java&type=git&repository=koyeb%2Fexample-java&branch=main&builder=buildpack&run_command=java+-jar+target%2Fexample-java-1.0-SNAPSHOT.jar&ports=8000%3Bhttp%3B%2F)

Clicking on this button brings you to the Koyeb App creation page with everything pre-set to launch this application.

_To modify this application example, you will need to fork this repository. Checkout the [fork and deploy](#fork-and-deploy-to-koyeb) instructions._

## Fork and deploy to Koyeb

If you want to customize and enhance this application, you need to fork this repository.

If you used the **Deploy to Koyeb** button, you can simply link your service to your forked repository to be able to push changes.  Alternatively, you can manually create the application as described below.

On the [Koyeb Control Panel](https://app.koyeb.com/), on the **Overview** tab, click the **Create Web Service** button to begin.

1. Select **GitHub** as the deployment method.
2. In the repositories list, select the repository you just forked.
3. Expand the **Builder** section and choose the builder you wish to use.  This repository can be built using buildpacks or a Dockerfile.
4. If building from a **buildpack**, click the **override** toggle associated with the **Run command** and enter `java -jar target/example-java-1.0-SNAPSHOT.jar` in the field.
5. Choose a name for your App and Service, i.e `java-on-koyeb`, and click **Deploy**.

You will be taken to the deployment page where you can follow the build of your Java application. Once the build is completed, your application will be deployed and you will be able to access it via `<YOUR_APP_NAME>-<YOUR_ORG_NAME>.koyeb.app`.

## Contributing

If you have any questions, ideas or suggestions regarding this application sample, feel free to open an [issue](https://github.com/koyeb/example-java/issues) or fork this repository and open a [pull request](https://github.com/koyeb/example-java/pulls).

## Contact

[Koyeb](https://www.koyeb.com) - [@gokoyeb](https://twitter.com/gokoyeb) - [Slack](http://slack.koyeb.com/)

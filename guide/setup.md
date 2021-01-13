---
description: "First of all, you will need to download the structure of the bot that will serve as a basis for your project. Follow carefully the contents below to avoid problems later on ! \U0001F680"
---

# Setup



### Download the framework

In the first time, clone the base repository

```
git clone https://github.com/discord-ts-app/discord-ts-app.git <project name>
```

{% hint style="info" %}
You can define the name of your project directly in the clone if you wish !
{% endhint %}



### Start your project

Then, the application must be initialized with the following three commands :

* Install the Node outbuildings
* Start the compilation of your bot in order to transcribe the typescript but javascript
* Start your bot

{% tabs %}
{% tab title="NPM" %}
```bash
npm install
```
{% endtab %}

{% tab title="YARN" %}
```
yarn install
```
{% endtab %}
{% endtabs %}

Now that the installation is done, you need to copy/paste the .env.example file, rename it to .env and modify its contents accordingly.

{% tabs %}
{% tab title="NPM" %}
```bash
npm run build
```
{% endtab %}

{% tab title="YARN" %}
```
yarn build
```
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="NPM" %}
```bash
npm run start
```
{% endtab %}

{% tab title="YARN" %}
```
yarn install
```
{% endtab %}
{% endtabs %}

{% hint style="warning" %}
You must use the last two commands at the same time, so open two ternimals in order to execute both commands.
{% endhint %}


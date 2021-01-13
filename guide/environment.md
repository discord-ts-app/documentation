# Environment



## Configure your bot is very easy

Go to the configurations folder of your application

### Environment file

You can configure your secret token and the prefor of your bot

{% code title=".env" %}
```text
CLIENT_PREFIX = "!"
SECRET_TOKEN = ""

# DIRECTORY
EVENTS_FOLDER = "Events"
COMMANDS_FOLDER = "Commands"
MIDDLEWARES_FOLDER = "Middlewares"
MODULES_FOLDER = "Modules"

# SETTINGS
DELETE_TIMEOUT_MESSAGE = 5000
NOT_ALLOW_EXECUTE_COMMAND = "You do not have permission to place this order."
```
{% endcode %}

### 

### Roles.ts

{% code title="App/Configurations/Roles.ts" %}
```typescript
enum Roles {
  // ROLE_NAME = 'role ID',
}

export default Roles
```
{% endcode %}

{% hint style="info" %}
To find roles id, please write in your discord chat `@\target_role`
{% endhint %}

### 

### Channels

{% code title="App/Configurations/Channels.ts" %}
```typescript
enum Channels {
  // CHANNEL_NAME = 'channel ID',
}

export default Channels
```
{% endcode %}

{% hint style="info" %}
To find channel id, please right click in our channel \(see more [here](https://support.discord.com/hc/fr/articles/206346498-O%C3%B9-trouver-l-ID-de-mon-compte-utilisateur-serveur-message-)\)
{% endhint %}



### Categories

{% code title="App/Configurations/Categories.ts" %}
```typescript
enum Categories {
  // CATEGORY_NAME = 'category ID',
}

export default Categories
```
{% endcode %}

{% hint style="info" %}
To find category id, it's same as channels id, please right click in our channel \(see more [here](https://support.discord.com/hc/fr/articles/206346498-O%C3%B9-trouver-l-ID-de-mon-compte-utilisateur-serveur-message-)\)
{% endhint %}


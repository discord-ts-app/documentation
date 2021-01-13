# Commands

Currently, the application does not offer a way to automatically generate event files. For this, you just have to create a typecript file in the `App/Commands/` folder and paste the code below :

```typescript
import { Command, CommandContext } from '@discord-ts-app/class-decorator'
import Roles from 'App/Configurations/Roles'
import { Message } from 'discord.js'

@Command({ name: 'Example', description: 'Description of example command', tag: 'example', alias: ['e'], roles: [Roles.EXAMPLE] })
export default class Example implements CommandContext {
	public async run(message: Message, args: string[]): Promise<void> {
		// Your code here
	}
}
```

That's it, nothing more is needed ! 😅


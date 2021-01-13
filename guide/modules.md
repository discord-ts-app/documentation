# Modules

Currently, the application does not offer a way to automatically generate event files. For this, you just have to create a typecript file in the `App/Modules/` folder and paste the code below :

```typescript
import { Event, Events, Command, Middleware, Lifecycles } from '@discord-ts-app/function-decorator'
import { Message } from 'discord.js'

export default class Module {
	@Event({ type: Events.MESSAGE })
	public async event(message: Message): Promise<void> {
		// Your code here
	}

	@Command({ name: 'Command', description: 'Description of command', tag: 'command', alias: ['c'] })
	public async command(message: Message, args: Array<string>): Promise<void> {
		// Your code here
	}

	@Middleware({ lifecycle: Lifecycles.MESSAGE_RECEIVED })
	public async middleware(): Promise<void> {
		// Your code here
	}
}

```

That's it, nothing more is needed ! 😅 


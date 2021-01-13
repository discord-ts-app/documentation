# Events

Currently, the application does not offer a way to automatically generate event files. For this, you just have to create a typecript file in the `App/Events/` folder and paste the code below :

```typescript
import { Event, Events, EventContext } from '@discord-ts-app/class-decorator'

@Event({ type: Events.READY }) // 👈 Choose your event here
export default class Example implements EventContext {
	public async run(): Promise<void> {
		// Your code here
	}
}
```

That's it, nothing more is needed ! 😅


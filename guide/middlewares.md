# Middlewares

Currently, the application does not offer a way to automatically generate event files. For this, you just have to create a typecript file in the `App/Middlewares/` folder and paste the code below :

```typescript
import { Middleware, MiddlewareContext } from '@discord-ts-app/class-decorator'

@Middleware('messageReceived') // 👈 Choose your lifecycle hook here
export default class Example implements MiddlewareContext {
	public async run(): Promise<void> {
		// Your code here
	}
}

```

That's it, nothing more is needed ! 😅 


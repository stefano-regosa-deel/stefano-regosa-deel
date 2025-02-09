
```typescript
import * as M from 'pattern-matching-ts/match'

const match = (about: About) =>
  pipe(
    about,
    M.matchW('_tag')({
       Name: () => 'Stefano Regosa',
       Role: () => 'Engineering team leader @ Deel',
       Blog: () => 'https://undefined.technology',
       Focus : () => ({ TypeScript , React , Node }),
       Currently: () => 'Hacking in TypeScript',
       AllAbout: () =>  ['writing software that runs at scale']
    })
  )
```

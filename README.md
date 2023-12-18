
```typescript
import * as M from 'pattern-matching-ts/match'

const match = (about: About) =>
  pipe(
    about,
    M.matchW('_tag')({
       Name: () => 'Stefano Regosa',
       Role: () => 'Senior Frontend Engineer @ Deel',
       Blog: () => 'https://undefined.technology',
       Focus : () => ({ TypeScript , React , Node }),
       Currently: () => 'Hacking in TypeScript',
       AllAbout: () =>  ['Open Source','Functional Programming','Clean code']
    })
  )
```

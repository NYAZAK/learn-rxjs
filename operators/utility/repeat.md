
# repeat

#### signature: `repeat(count: number): Observable`

## Repeats the stream of items emitted by the source Observable at most count times.

<div class="ua-ad"><a href="https://ultimatecourses.com/?ref=76683_kee7y7vk"><img src="https://ultimatecourses.com/assets/img/banners/ultimate-angular-leader.svg" style="width:100%;max-width:100%"></a></div>

### Examples

##### Example 1: Repeat 3 times

(
[StackBlitz](https://stackblitz.com/edit/rxjs-repeat-learnrxjs?file=index.ts&devtoolsheight=100) )

```js
// RxJS v6+
import { repeat, delay } from 'rxjs/operators';
import { of } from 'rxjs';

const delayedThing = of('delayed value').pipe(delay(2000));

delayedThing.pipe(
  repeat(3)
)
.subscribe(console.log)

```

### Related Recipes

- [Lockscreen](../../recipes/lockscreen.md)

### Additional Resources

- [repeat](http://reactivex.io/rxjs/class/es6/Observable.js~Observable.html#instance-method-repeat)
  :newspaper: - Official docs

---

> :file_folder: Source Code:
> [https://github.com/ReactiveX/rxjs/blob/master/src/internal/operators/repeat.ts](https://github.com/ReactiveX/rxjs/blob/master/src/internal/operators/repeat.ts)

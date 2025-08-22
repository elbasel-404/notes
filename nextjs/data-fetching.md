utilize `Promise.all()` and `Promise.allSettled()` to run fetch requests in parallel 
and avoid using multiple async/await fetch calls sequentially as this will result in
the blockage of rendering as a request won't run until the prev one has finished.

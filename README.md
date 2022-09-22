`flutter run`

If you click on the following, in this sequence:

- The "A Screen" Tab
- The "View A Details" link
- Back navigation arrow
- The "B Screen" Tab
- The "View B Details" link
- Back navigation arrow

Then the only things that are logged are:

```
[MyNavObserver] didPush: route(: {}), previousRoute= null
[MyNavObserver] didPush: route(/b/details: {}), previousRoute= route(: {})
[MyNavObserver] didPop: route(/b/details: {}), previousRoute= route(: {})
```

Even though all navigation was through things like `GoRouter.of(context).go('/a')`

The only route that appears as part `NavigatorObserver` is the `b/details` route, and I wonder if it's because it's using a `_rootNavigatorKey`.

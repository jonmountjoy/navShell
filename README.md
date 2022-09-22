`flutter run`

When going to page 2:

```
[INFO] GoRouter: going to /page2/pv1?q1=qv1
[INFO] MyNavObserver: didPush: route(page2: {p1: pv1, q1: qv1}), previousRoute= route(/: {q1: qv1})
[INFO] MyNavObserver: didPop: route(page2: {p1: pv1, q1: qv1}), previousRoute= route(/: {q1: qv1})
```

When going to page 2 alternative:

```
[INFO] GoRouter: going to /page2alternative/pv1?q1=qv1
[INFO] MyNavObserver: didPush: route(null: null), previousRoute= route(/: {q1: qv1})
[INFO] MyNavObserver: didPop: route(null: null), previousRoute= route(/: {q1: qv1})
```

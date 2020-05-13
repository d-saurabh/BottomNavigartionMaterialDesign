# Bottom Navigation Menu

- add `implementation 'com.google.android.material:material:1.2.0-alpha06'` to app gradle
- Under the `res` create a new `resource directory` called `menu`
- Create items using `item` tag
- On your `activity_main` add `bottomNavigationView` which comes with the material library
- Use following to change the content when each menu clicked
```
    bottomNavigationView.setOnNavigationItemSelectedListener {
        true
    }
```
- Use the following to add badges on the menu items
```
    bottomNavigationView.getOrCreateBadge(R.id.miMessages).apply{
        number = 10
        isVisible = true
    }
```

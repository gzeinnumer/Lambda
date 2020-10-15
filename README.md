# Lambda

- Active Lambda by add code in `Gradle`.
> Java
```gradle
android {

    ...
    
    compileOptions {
        sourceCompatibility JavaVersion.VERSION_1_8
        targetCompatibility JavaVersion.VERSION_1_8
    }
}

dependencies {
    ...
}
```

>Kotlin
```gradle
android {
    
    ...
    
    compileOptions {
        sourceCompatibility JavaVersion.VERSION_1_8
        targetCompatibility JavaVersion.VERSION_1_8
    }
    kotlinOptions {
        jvmTarget = '1.8'
    }
}

dependencies {
    ...
}
```

- Sample code.
```java
//without Lambda
button.setOnClickListener(new View.OnClickListener() {
    @Override
    public void onClick(View v) {

    }
});

with Lambda
button.setOnClickListener(v -> {

});
```

---

```
Copyright 2020 M. Fadli Zein
```
### 035-Optional Chaining ?.

* It is the safest way to access nested object properties.

```
let userAdmincheck = {
  admin() {
  console.log("i am chaining check admin")
  }
};

let userGuest = {}
userAdmincheck.admin?.();
userGuest.admin?.();
userGuest.admin;
```
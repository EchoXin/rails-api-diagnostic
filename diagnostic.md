# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
get the request from the client and return the data back to client.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
model
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
controller
```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
index, show, create, update, destroy, new, edit
```

A user action fires a `PATCH` request for `pets/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list,
please include information on dynamic segments, the params hash and seralizers).

```bash
Route get the request and send it to controller
Controller ask model to fetch the first pet from database.
Model return the first pet.
Seralizers return the data by json to the controller.
Controller excute update action using the first pet as param.


```

What is the command to scaffold a `medicalRecords` join table which holds
refrences to a `pets` and a `vets` table?

```bash
rails g scaffold MedicalRecord pet:references vet:references
```

What is the point of having a join table?

```bash
To connect two tables with many-to-many relationship.
```

Give an example of a one-to-many relationship and a many-to-many relationship:

```bash
one user can have many diaries, but one diary only belong to one user.
a student has many teachers and a teacher has many students.
```



# TypeScript

## 📘 Overview

This project introduces **TypeScript**, a typed superset of JavaScript that helps developers write cleaner, more maintainable, and less error-prone code.
You’ll learn how to use interfaces, classes, functions, generics, namespaces, declaration merging, and more — all while working with the DOM and building modular TypeScript applications compiled with Webpack.

---

## 🧠 Learning Objectives

By the end of this project, you should be able to explain (without Google):

* Basic types in TypeScript
* How to define and use **interfaces**, **classes**, and **functions**
* How to interact with the **DOM** using TypeScript
* How to use **generic types**
* How to organize code using **namespaces**
* How **declaration merging** works
* How to use an **ambient namespace** to import an external library
* How to implement **nominal typing** in TypeScript

---

## ⚙️ Requirements

* Allowed editors: `vi`, `vim`, `emacs`, `Visual Studio Code`
* All files should end with a new line
* All code should compile and run on **Ubuntu 18.04 LTS**
* TypeScript code will be checked with **Jest (v24.9.*)**
* Each TypeScript file must use the `.ts` extension
* TypeScript compiler must show **no warnings or errors** when building
* A `README.md` file is mandatory at the root of the project

---

## 🧩 Project Structure

```
0x04-TypeScript/
│
├── task_0/
│   ├── js/main.ts
│   ├── package.json
│   ├── tsconfig.json
│   ├── webpack.config.js
│   └── .eslintrc.js
│
├── task_1/
│   ├── js/main.ts
│   ├── package.json
│   ├── tsconfig.json
│   └── webpack.config.js
│
├── task_2/
│   ├── js/main.ts
│   ├── package.json
│   ├── tsconfig.json
│   └── webpack.config.js
│
├── task_3/
│   ├── js/main.ts
│   ├── js/interface.ts
│   ├── js/crud.d.ts
│   ├── js/crud.js
│   ├── package.json
│   ├── tsconfig.json
│   └── webpack.config.js
│
├── task_4/
│   ├── js/main.ts
│   ├── js/subjects/
│   │   ├── Cpp.ts
│   │   ├── Java.ts
│   │   ├── React.ts
│   │   ├── Subject.ts
│   │   └── Teacher.ts
│   ├── package.json
│   └── tsconfig.json
│
└── task_5/
    ├── js/main.ts
    ├── package.json
    ├── tsconfig.json
    └── webpack.config.js
```

---

## 🧱 Tasks Summary

### **Task 0: Creating an interface for a student**

* Create a `Student` interface with `firstName`, `lastName`, `age`, and `location`.
* Render an HTML table showing each student’s first name and location.
* Use TypeScript everywhere and compile with Webpack (no errors).

---

### **Task 1: Teacher interface**

* Define a `Teacher` interface with:

  * `firstName` and `lastName` (readonly)
  * `fullTimeEmployee` (boolean)
  * `yearsOfExperience` (optional)
  * `location` (string)
  * `[key: string]: any` (to allow additional properties)
* Extend it with a `Directors` interface adding `numberOfReports`.
* Implement a `printTeacher` function and `StudentClass` class using interfaces.

---

### **Task 2: Advanced types**

* Create `DirectorInterface` and `TeacherInterface` with specific methods.
* Implement `Director` and `Teacher` classes.
* Write a function `createEmployee` returning either `Director` or `Teacher` based on salary.
* Add `isDirector` type predicate and `executeWork` function.
* Create a `Subjects` string literal type (`"Math" | "History"`) and a `teachClass` function.

---

### **Task 3: Ambient Namespaces**

* Create a `RowID` type and `RowElement` interface.
* Write an ambient declaration file `crud.d.ts` for external library `crud.js`.
* Use the `CRUD` module to insert, update, and delete rows, with TypeScript typing.

---

### **Task 4: Namespaces & Declaration Merging**

* Create a `Subjects` namespace with:

  * `Teacher` interface
  * `Subject` base class
  * Specialized classes `Cpp`, `Java`, and `React`
* Use declaration merging to extend `Teacher` for each language.
* Implement `getRequirements()` and `getAvailableTeacher()` methods.
* In `main.ts`, log each subject’s information and teacher availability.

---

### **Task 5: Brand Convention & Nominal Typing**

* Create interfaces `MajorCredits` and `MinorCredits` with unique brand properties.
* Implement `sumMajorCredits()` and `sumMinorCredits()` to sum subject credits while maintaining distinct nominal types.

---

## 🧰 Configuration Files

Each task folder contains:

* **`package.json`** — Project dependencies and build scripts
* **`tsconfig.json`** — TypeScript compiler options
* **`webpack.config.js`** — Bundler configuration
* **`.eslintrc.js`** (only in Task 0) — Linting rules

---

## 🏗️ Build & Run

### Install dependencies:

```bash
npm install
```

### Build project:

```bash
npm run build
```

### Start dev server (where applicable):

```bash
npm start
```

When you build, TypeScript should output:

```
No type errors found.
```

---

## 🧑‍💻 Author

**ALX Frontend JavaScript — TypeScript Module**

Developed as part of the **ALX Frontend Specialization** curriculum.


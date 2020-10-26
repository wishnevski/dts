
<!-- ------------------------ TABLE OF CONTENTS ------------------------ -->


# Table of Contents

- [DTS](#dts)
- [Example](#example)
  - [Without DTS](#arbitrary-code-without-using-dts)
  - [With DTS](#arbitrary-code-using-dts)
- [Documentation](#documentation)
  - [Long desh](#long-desh)
  - [Normal desh](#normal-desh)
  - [Short desh](#short-desh)
  - [Small desh](#small-desh)


<!-- ------------------------ DTS ------------------------ -->


# DTS


**DTS** *(Dash Two Spaces)* is a universal code splitting methodology through comments for all popular programming languages, the main purpose of which is to increase readability.

The basic concept is simple: the semantic parts of the code are separated by dashes *(single line comments consisting of dashes)*, surrounded by spaces *(two blank lines at the top and bottom)*.

Dashes have different accent characteristics, which allows dividing the code into nested hierarchies, as well as naming parts of the code, making it easier to visually find the necessary pieces.

In this repository you can find a file with a list of existing deshes for your specific language. It will be named `DTS.<Your language file extension>`. E.g. `DTS.js` or `DTS.cpp` etc.


<!-- ------------------------ EXAMPLE ------------------------ -->


# Example


*The examples use **JavaScript** syntax, but the methodology can be used in all languages that support single-line comments.*


#### Arbitrary code without using **DTS**:


```javascript
function Player()
{
  this.health = 100;
  this.armor = 0;
  this.buff = 0;


  this.position = { x: 0, y: 0, z: 0 };
  this.speed = { x: 0, y: 0, z: 0 };
  this.look = { x: 0, y: 0, z: 0 };


  this.move = function(direction, speed)
  {
    // do something
  }


  this.jump = function(height)
  {
    // do something
  }


  this.heal = function(value)
  {
    // do something
  }


  this.kill = function()
  {
    // do something
  }
}
```


#### Arbitrary code using **DTS**:


```javascript
function Player()
{
  this.health = 100;
  this.armor = 0;
  this.buff = null;

  this.position = { x: 0, y: 0, z: 0 };
  this.speed = { x: 0, y: 0, z: 0 };
  this.look = { x: 0, y: 0, z: 0 };


  /* ------------------------------------------------------ */
  /* ------------------------------------------------------ */


  this.move = function(direction, speed)
  {
    // do something
  }


  /* ---------------------------- */


  this.jump = function(height)
  {
    // do something
  }


  /* ---------------------------- */


  this.heal = function(value)
  {
    // do something
  }


  /* ---------------------------- */


  this.kill = function()
  {
    // do something
  }
}
```


Note, that two blank lines above and below desh are required condition, not one.


<!-- ------------------------ DOCUMENTATION ------------------------ -->


# Documentation


## Long desh


Triple named:

```javascript
/* ----------------------------------------------------------------------------------------------------------- */
/* -------------------------------------------------- TITLE -------------------------------------------------- */
/* ----------------------------------------------------------------------------------------------------------- */
```

Triple:

```javascript
/* ------------------------------------------------------------------------------------------------------------ */
/* ------------------------------------------------------------------------------------------------------------ */
/* ------------------------------------------------------------------------------------------------------------ */
```

Double:

```javascript
/* ------------------------------------------------------------------------------------------------------------ */
/* ------------------------------------------------------------------------------------------------------------ */
```

Single:

```javascript
/* ------------------------------------------------------------------------------------------------------------ */
```

Single named:

```javascript
/* --------------------------------------------------- TITLE --------------------------------------------------- */
```


## Normal desh


Triple named:

```javascript
/* ------------------------------------------------------- */
/* ------------------------ TITLE ------------------------ */
/* ------------------------------------------------------- */
```

Triple:

```javascript
/* ------------------------------------------------------ */
/* ------------------------------------------------------ */
/* ------------------------------------------------------ */
```

Double:

```javascript
/* ------------------------------------------------------ */
/* ------------------------------------------------------ */
```

Single:

```javascript
/* ------------------------------------------------------ */
```

Single named:

```javascript
/* ------------------------ TITLE ------------------------ */
```


## Short desh


Triple:

```javascript
/* ---------------------------- */
/* ---------------------------- */
/* ---------------------------- */
```

Double:

```javascript
/* ---------------------------- */
/* ---------------------------- */
```

Single:

```javascript
/* ---------------------------- */
```

Single named:

```javascript
/* ----------- TITLE ----------- */
```


## Small desh


Single:

```javascript
/* TITLE */
```

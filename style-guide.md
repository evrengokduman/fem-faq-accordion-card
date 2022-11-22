# Front-end Style Guide

## Layout

The designs were created to the following widths:

- Mobile: 375px
- Desktop: 1440px


:root {
  --dark-blue: hsl(238, 29%, 16%);
  --Soft-red: hsl(14, 88%, 65%);
  /*gradient*/
  --soft-violet: hsl(273, 75%, 66%);
  --soft-blue: hsl(240, 73%, 65%);
  /*text*/
  --dark-grayish-blue: hsl(237, 12%, 33%);
  --grayish-blue: hsl(240, 6%, 50%);

  /*dividers*/
  --light-grayish-blue: hsl(240, 5%, 91%);
  --kumbh-font: "Kumbh Sans", sans-serif;
}

html {
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

body {
  min-height: 100vh;
  margin: 0;
  padding: 3rem;
  font-family: var(--kumbh-font);
  background-image: linear-gradient(var(--soft-violet), var(--soft-blue));
}

/*MOBILE and general*/
.card {
  background-color: #ffff;
  border-radius: 2rem;
  max-width: 56rem;
  margin: 3rem auto;
}

.card__box {
  display: none;
}

.card__image img {
  width: 100%;
  height: auto;
  max-width: 25rem;
}

.card__text {
}

/*DESKTOP*/
@media (min-width: 56em) {
  .card {
    display: flex;
    margin: 6rem auto;
    padding-right: 2rem;
    background-image: url("/images/bg-pattern-desktop.svg");
    background-size: 45%;
    background-repeat: no-repeat;
    background-position: -13% center;
  }

  .card__box {
    display: block;
    position: absolute;
    z-index: 1;
    top: 50%;
    left: 0;
    transform: translateX(-50%), translateY(-50%);
  }
  .card__image,
  .card__text {
    flex: 1;
  }

  .card__image {
    display: flex;
    align-items: center;

    overflow: hidden;
  }
  .card__image img {
    transform: translateX(-4rem);
  }
}

## Colors

### Primary

#### Text

- Very dark desaturated blue: hsl(238, 29%, 16%)
- Soft red: hsl(14, 88%, 65%)

#### Gradient

Background gradient:

- Soft violet: hsl(273, 75%, 66%)
- Soft blue: hsl(240, 73%, 65%)

### Neutral

#### Text

- Very dark grayish blue: hsl(237, 12%, 33%)
- Dark grayish blue: hsl(240, 6%, 50%)

#### Dividers

- Light grayish blue: hsl(240, 5%, 91%)

## Typography

### Body Copy

- Font size: 12px

### Font

- Family: [Kumbh Sans](https://fonts.google.com/specimen/Kumbh+Sans)
- Weights: 400, 700

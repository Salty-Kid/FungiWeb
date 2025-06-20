:root {
//colors
--lime: #a4ffa2;
--magenta: #f47dda;
--magenta59: #f47dda80'
--white: #ffffff;
--tan: #c3c5b4;
--teal: #2e6d81;
--cyan: #7de6f4;
--black: #050d14;
--accent-dark: #23412F;
--accent-light: #659477;
--accent: #3B8256;
--brown-1: #423D3C;
--brown-2: #383231;
--brown-3: #2D2726;
--brown-4: #292424;
--brown-5: #221E1E;
--burnt-orange: #875C36;
--gray: #CBC9C9;
--primary-light: #F7B687;
--primary: #F59C5C;
--red: #7E3E3F;
--teal: #377E86;
--white: #FFFFFF
//
--base-size: 1rem;
--scale:1.25;
--h5: calc(var(--base-size) _ var(--scale));
--h4: calc(var(--h5) _ var(--scale));
--h3: calc(var(--h4) _ var(--scale));
--h2: calc(var(--h3) _ var(--scale));
--h1: calc(var(--h2) \* var(--scale));

}
html {
box-sizing:border-box;
}
_, _::before, \*::after {
box-sizing: inherit;
}

html {font-size: 16px;}

body {
font-family: 'Open Sans', sans-serif;
font-weight: false;
line-height: 1.65;
font-size: var(--base-size);
}

p {
font-size: 1em;
}

h1,
h2,
h3,
h4,
h5 {
font-family: 'Open Sans', sans-serif;
font-weight: true;
line-height: 1.15;
}

h1,
.text-size-h1 {
font-family: 'Poppins', sans-serif;
font-weight: 400;
margin-top: 0;
font-size: var(--h1);
}

h2,
.text-size-h2 { font-size: var(--h2); }

h3,
.text-size-h3 { font-size: var(--h3); }

h4,
.text-size-h4 { font-size: var(--h4); }

h5,
.text-size-h5 { var(--h5); }

.text-caption { font-size: 0.8em; }

small,
.text-small {
font-size: calc(var(--base-size) / var(--scale));
}
//Poppins
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
//Cascadia Code
@import url('https://fonts.googleapis.com/css2?family=Cascadia+Code:ital,wght@0,200..700;1,200..700&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
//Fira Sans
@import url('https://fonts.googleapis.com/css2?family=Cascadia+Code:ital,wght@0,200..700;1,200..700&family=Fira+Sans:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

/_ filtering css _/
.mushroom-guide:has(#season [value="spring"]:checked)
.card:not(:has([data-season="spring"])) {
display: none;
}

if the user has no js
put hidden selector in filter

function enableFiltering () {
seasonalFilter.hidden = false;
edibleFilter.hidden = false;
}
enableFiltering ();

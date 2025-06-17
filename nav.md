[aria-controls="primary-nav"] {
z-index: 100;
background: transparent;
border: 0;
cursor: pointer;

    img {
      border-radius: 0;
    }

}

.primary-navigation {
ul {
display: flex;
flex-wrap: wrap;
gap: 0.5rem 1rem;
}
@media (width < 760px) {
background-color: var(--background-accent-main);
padding: 2rem;
position: absolute;
z-index: 10;
top: 0;
right: 0;
font-size: --font-size-lg;
font-family: var(--ff-heading);
font-weight: 700;
border-radius: 0 0 0 var(--border-radius-3);

      ul {
        gap: 0;
        flex-direction: column;
      }
      li + li {
        margin-block-start: 1.5rem;
        padding-block-start: 1.5rem;
        border-top: 2px solid var(--background-accent-light);
      }
    }

}

JS CODE

 <!--NAVIGATION EXAMPLE HTML LAYOUT
 ONLY ON MOBILE DESIGN-->

 <header class="site-header">
      <div class="wrapper" data-width="wide">
        <div class="site-header__inner">
          <img src="assets/fungi-finders.svg" alt="logo" />
          <button aria-controls="primary-nav" aria-expanded="false">
            <img src="assets/hamburger.svg" alt="button for other pages" />
          </button>
          <nav id="primary-nav" class="primary-navigation">
            <ul role="lists">
              <li><a href="/">Discover</a></li>
              <li><a href="#">Mushroom Guide</a></li>
              <li><a href="#">FAQ</a></li>
            </ul>
          </nav>
        </div>
      </div>
    </header>

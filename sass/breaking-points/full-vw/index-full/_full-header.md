.header-flex {
    @include display;
    align-items: center;
  }
  .header-flex-logo {
    @include display;
    @include list;
    margin-right: 93px;
  
    @media screen and (min-width: 768px) {
      padding-top: 16px;
      padding-bottom: 16px;
      margin: 0;
    }
  }
  .header-flex-nav {
    @include list($margin: none);
  
    & .mr-li + .mr-li {
      margin-left: 50px;
    }
  
    @media screen and (min-width: 1200px) {
        @include display;
        margin-left: 93px;
    }
  }
  .header-nav {
    position: relative;
    @include list($margin: none, $padding: none);
  
    &:hover,
    &:focus {
      color: $accent-color;
    }
    & {
      padding-top: 32px;
      padding-bottom: 32px;
      transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);
    }
    & {
      font-family: $font-main;
      font-size: 14px;
      font-weight: 500;
      line-height: 1.14;
      letter-spacing: 0.02em;
      color: $main-text-color;
    }
  
    @media screen and (min-width: 768px) {
      display: block;
    }
  }
  .header-navigation-button {
    padding-top: 10px;
    padding-bottom: 10px;
    margin-left: auto;
    justify-content: flex-end;
    transition: fill 250ms cubic-bezier(0.4, 0, 0.2, 1);
  
    &:hover {
      fill: $accent-color;
    }
  
    @media screen and (min-width: 768px) {
      display: none;
    }
  }
  .mobile-menu.is-open {
    display: block;
  }
  .mobile-menu {
    display: none;
  }
  .mr-li:nth-child(1) .header-nav::after {
    content: "";
    position: absolute;
    left: 0;
    bottom: -1px;
    display: block;
    border-radius: 2px;
    width: 100%;
    height: 4px;
    background-color: $accent-color;
  }
  .mr-li:nth-child(1) .header-nav {
    color: $accent-color;
  }
  .header-flex-contact {
      flex-direction: column;
    @include list;
    margin-left: auto;
  
    @media screen and (min-width: 1200px) {
        @include display;
        flex-direction: row;
    }
  }
  .header-contact {
    @include list($margin: none, $padding: none);
    align-items: center;
  
    & {
      transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);
    }
    &:hover,
    &:focus {
      color: $accent-color;
    }
    @media screen and (min-width: 1200px) {
        @include display;
        margin-bottom: 0px;
        margin-right: 30px;
        padding-top: 32px;
        padding-bottom: 32px;
    }
  }
  .mr-li:nth-child(2) .header-contact {
      margin-bottom: 0;

      @media screen and (min-width: 1200px) {
        margin-right: 0;
      }
  }
  .links-icon {
    margin-right: 10px;
    fill: currentColor;
  }
  .header-contact {
    font-family: $font-main;
    font-weight: 500;
    font-size: 12px;
    line-height: 14px;
    letter-spacing: 0.02em;
    color: $second-color;

    @media screen and (min-width: 1200px) {
      font-size: 14px;
      line-height: 16px;
  }
}
  .header-logo-second-color {
    font-family: $font-logo;
    font-weight: bold;
    font-size: 26px;
    line-height: 1.2;
    color: $main-text-color;
  }
  .header-logo-first-color {
    color: $accent-color;
  }
  
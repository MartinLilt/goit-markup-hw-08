.mobile-menu {
  position: fixed;
  top: 0;
  left: 0;
  overflow-y: scroll;
  width: 100%;
  height: 100%;
  background-color: $core-color;
  z-index: 999;
}

.mobile-menu .content {
  padding: 0px 40px 48px 40px;
}
.close-menu-help {
  margin-right: 15px;
}
.mobile-navigation-button {
  padding-top: 10px;
  padding-bottom: 10px;
  margin-left: auto;
  display: flex;
  justify-content: flex-end;
  transition: fill 250ms cubic-bezier(0.4, 0, 0.2, 1);

  &:hover {
    fill: $accent-color;
  }
}
.icon-close {
  display: inline;
}
.navigation {
  @include list($margin: none);
  margin-bottom: 302px;
  margin-top: 0px;
}
.navigation-category {
  @include list;
  transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);

  &:hover {
    color: $accent-color;
  }

  &:not(:last-child) {
    margin-bottom: 32px;
  }
}
.contact {
  margin-bottom: 64px;
  transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);

  &:hover {
    color: $accent-color;
  }
}
.contact-category {
  @include list;

  &:not(:last-child) {
    margin-bottom: 32px;
  }
}
.social {
  @include list;
  @include display;
  flex-wrap: wrap;
}
.social-drob {
  height: 22px;
  width: 1px;
  background-color: rgba(33, 33, 33, 0.2);
  margin-left: 10px;
  margin-right: 10px;
  display: flex;
}
.social-link {
  @include list;
  font-family: $font-main;
font-weight: 500;
font-size: 18px;
line-height: 1.22;
letter-spacing: 0.02em;
color: $accent-color;
}
.navigation-category {
  @include list($margin: none);
font-family: $font-main;
font-weight: 500;
font-size: 40px;
line-height: 1.17;
letter-spacing: 0.02em;
color: $main-text-color;
}

.mobile-menu .accent-contact {
  @include list;
  font-family: $font-main;
font-weight: 500;
font-size: 34px;
line-height: 40px;
letter-spacing: 0.02em;
color: $accent-color;
}

.contact {
  @include list($margin: none);
  font-family: $font-main;
font-weight: 500;
font-size: 24px;
line-height: 28px;
letter-spacing: 0.02em;
color: $second-color;
}
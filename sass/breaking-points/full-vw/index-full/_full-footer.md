.footer-background_container {
  background: $background-second-cl;
}
.footer-social_flex {
  @include display;
  justify-content: center;
  @include list;
}
.footer-flex_container {
  @include list;

  @media screen and (min-width: 768px) {
    @include display;
    flex-wrap: wrap;
  }
}
.footer_logo-second_color {
  @include list;
  display: block;
  margin-bottom: 20px;
  text-align: center;

  @media screen and (min-width: 768px) {
    text-align: start;
  }
}
.footer-contacts {
  @include list;
  text-align: center;

  @media screen and (min-width: 768px) {
    text-align: start;
  }
}
.footer-links {
  @include list;
  margin-bottom: 10px;
  display: block;
}
.footer-links {
  transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);

  &:hover,
  &:focus {
    color: $accent-color;
  }
}
.footer-links {
  font-family: $font-main;
  font-weight: normal;
  font-size: 14px;
  line-height: 1.71;
  color: rgba(255, 255, 255, 0.6);
}
.footer_logo-second_color {
  font-family: $font-logo;
  font-weight: bold;
  font-size: 26px;
  line-height: 1.19;
  color: $core-color;
}
.footer_logo-first_color {
  color: $accent-color;
}
.footer-address_box {
  margin-bottom: 60px;

  @media screen and (min-width: 1200px) {
    margin-bottom: 0;
    margin-right: 70px;
    margin-left: 0;
  }
}
.footer-address {
  margin-bottom: 10px;
  text-align: center;
}
.footer-social_box {
  text-align: center;
  margin-bottom: 60px;

  @media screen and (min-width: 1200px) {
    text-align: start;
    margin-bottom: auto;
    margin-left: 0;
    margin-right: 93px;
  }
}
.footer-social_title {
  margin: 12px 0px 20px 0px;

  @media screen and (min-width: 768px) {
    margin: 0px 0px 20px 0px;
  }
}
.footer-social_link {
  @include list;
  margin-right: 10px;

  &:nth-child(4n) {
    margin-right: 0px;
  }
}
.footer-social {
  @include display;
  padding: 12px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.1);
  fill: $core-color;

  &:hover,
  &:focus {
    background-color: $accent-color;
    fill: $background-core-cl;
  }
}
.footer-social {
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
    fill 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.footer-social_title {
  font-family: $font-main;
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;
  text-transform: uppercase;
  color: $core-color;
}
.footer-address {
  font-style: inherit;
  font-family: $font-main;
  font-weight: normal;
  font-size: 14px;
  line-height: 1.71;
  letter-spacing: 0.03em;
  color: $core-color;
}
.footer-lead {
  @include display;
  flex-direction: column;
  justify-content: center;
  
  @media screen and (min-width: 1200px) {
    flex-direction: column;
    justify-content: flex-start;
    margin-left: 0;
    margin-right: 0;
  }
}
.footer-lead_form {
  @include display;
  flex-direction: column;
  justify-content: center;

  @media screen and (min-width: 1200px) {
    justify-content: flex-start;
    flex-direction: row;
  }
}
.footer-lead_text {
  text-align: center;
  margin: 12px 0px 20px 0px;

  @media screen and (min-width: 1200px) {
    text-align: start;
    margin: 0px 0px 20px 0px;
  }
}
.footer-lead_text {
  font-family: $font-main;
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;
  text-transform: uppercase;
  color: $core-color;
}
.footer-lead_field {
  @include display;
  justify-content: center;
  margin-bottom: 20px;

  @media screen and (min-width: 1200px) {
    margin-bottom: 0;
  }
}
.footer-lead_input {
  padding-left: 16px;
  height: 50px;
  width: 100%;
  outline: none;

  &:focus {
    border: 1px solid $accent-color;
  }
  &::placeholder {
    font-family: $accent-color;
    font-weight: normal;
    font-size: 16px;
    line-height: 1.25;
    color: rgba(255, 255, 255, 0.6);
  }

  @media screen and (min-width: 1200px) {
    width: 373px;
    margin-right: 12px;
  }
}
.footer-lead_input {
  color: rgba(255, 255, 255, 0.6);
  background-color: rgba(0, 0, 0, 0);
  border: 1px solid rgba(255, 255, 255, 0.3);
  filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.15));
  border-radius: 4px;
}
.footer-button_box {
  @include display;
  justify-content: center;

  @media screen and (min-width: 1200px) {
    justify-content: flex-start;
  }
}
.footer-button {
  width: 200px;
  @include button-style;
  padding: 10px 28px 10px 28px;
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1);

  &:hover {
    background-color: $accent-hover-button;
  }
}
.footer-button_svg {
  @include display;
  margin-left: 11px;
  fill: $core-color;
}

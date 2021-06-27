.regular_customers-flex_container {
  @include display;
  @include list;
  flex-wrap: wrap;

  @media screen and (min-width: 320px) {
    justify-content: center;
  }
}
.regular_customers-title {
  text-align: center;
  margin: 0px 0px 50px 0px;
}
.regular_customers-box:nth-child(2n+1) {
  @media screen and (min-width: 480px) {
    margin-right: 30px;
  }
}
.regular_customers-box:nth-child(n+5) {
  @media screen and (min-width: 480px) {
    margin-bottom: 0;
  }
}
.regular_customers-box {
  @media screen and (min-width: 320px) {
    margin-bottom: 30px;
  }
}
.regular_customers-box:nth-child(n+6) {
  @media screen and (min-width: 320px) {
    margin-bottom: 0;
  }
}
.regular_customers-social {
  @include display;
  border-radius: 4px;
  border: 1px solid $background-icon-team;
  fill: $background-icon-team;
  transition: border 250ms cubic-bezier(0.4, 0, 0.2, 1),
    fill 250ms cubic-bezier(0.4, 0, 0.2, 1);

  &:hover,
  &:focus {
    fill: $accent-color;
    border: 1px solid $accent-color;
  }
  @media screen and (min-width: 320px) {
    padding: 15px 91px 15px 91px;
  }
  @media screen and (min-width: 480px) {
    padding: 15px 51px 15px 51px;
  }
}
.regular_customers-title {
  font-family: $font-main;
  font-style: normal;
  font-weight: bold;
  font-size: 28px;
  line-height: 33px;
  letter-spacing: 0.03em;
  color: $main-text-color;
}
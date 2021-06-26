.hero_menu-container {
  margin-left: auto;
  margin-right: auto;
  background: $background-second-cl;
  background-image: linear-gradient(
      to right,
      rgba(47, 48, 58, 0.4),
      rgba(47, 48, 58, 0.4)
    ),
    url('core-bg-mobile.webp');
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;

  @media screen and (min-width: 320px) {
    padding-top: 118px;
    padding-bottom: 118px;
  }

  @media (min-device-pixel-ratio: 2),
  (-webkit-min-device-pixel-ratio: 2),
  (min-resolution: 192dpi),
  (min-resolution: 2dppx) {
  .hero_menu-container {
    background-image: linear-gradient(
      to right,
      rgba(47, 48, 58, 0.4),
      rgba(47, 48, 58, 0.4)
    ),
    url('core-bg-mobile2x.webp');
  }
}
}
.hero_menu-core_text {
  text-align: center;
  margin: 0px 0px 30px 0px;

  @media screen and (min-width: 320px) {
    font-family: $font-main;
    font-style: normal;
    font-weight: 900;
    font-size: 26px;
    line-height: 1.62;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    color: $core-color;
  }
}
.hero_menu-core_button {
  margin-left: auto;
  margin-right: auto;
  padding: 10px 32px 10px 32px;
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1);
  @include button-style;

  &:hover {
    background-color: $accent-hover-button;
  }
}

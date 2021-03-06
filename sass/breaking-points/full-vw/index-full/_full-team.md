.our_team-background_container {
  background: $background-ourteam-cl;
}
.our_team-title {
  text-align: center;
  margin: 0px 0px 50px 0px;
}
.our_team-flex_container {
  @include list;

  @media screen and (min-width: 768px) {
    @include display;
    flex-wrap: wrap;
  }
}
.our_team-box:nth-child(n+4) {
  @media screen and (min-width: 1200px) {
    margin-right: 0;
  }
}
.our_team-box:nth-child(n+1) {
  @media screen and (min-width: 1200px) {
    margin-bottom: 0;
  }
}
.our_team-box {
  text-align: center;
  margin-bottom: 30px;

  @media screen and (min-width: 1200px) {
    width: 270px;
    margin-right: 30px;
  }
}
.our_team-img {
  width: 100%;
}
.our_team-box:nth-child(4) {
  margin-bottom: 0;
}
.our_team-link_box {
  padding: 30px 32px 30px 32px;
}
.our_team-link_title {
  text-align: center;
  margin: 0px 0px 10px 0px;
}
.our_team-link_text {
  text-align: center;
  margin: 0px 0px 16px 0px;
}
.our_team-flex_link {
  @include display;
  @include list;
  flex-wrap: wrap;
  justify-content: center;
}
.our_team-social_box {
  @include list;
  margin-right: 10px;

  &:nth-child(4n) {
    margin-right: 0px;
  }
}
.our_team-social {
  @include display;
  padding: 12px;
  border-radius: 50%;
  fill: $background-icon-team;
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
    fill 250ms cubic-bezier(0.4, 0, 0.2, 1);

  &:hover,
  &:focus {
    background-color: $accent-color;
    fill: $background-core-cl;
  }
}
.our_team-svg {
  @include display;
}
.our_team-link_text {
  font-family: $font-main;
  font-weight: normal;
  font-size: 16px;
  line-height: 1.19;
  color: $second-color;
}
.our_team-link_title {
  font-family: $font-main;
  font-size: 16px;
  font-weight: 500;
  line-height: 1.19;
  color: $main-text-color;
}
.our_team-title {
  font-family: $font-main;
  font-style: normal;
  font-weight: bold;
  font-size: 28px;
  line-height: 33px;
  text-align: center;
  letter-spacing: 0.03em;
  color: $main-text-color;
}
.our_team-box {
  background: $background-core-cl;
  box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.12), 0px 1px 1px rgba(0, 0, 0, 0.14),
    0px 2px 1px rgba(0, 0, 0, 0.2);
  border-radius: 0px 0px 4px 4px;
}

.visually-hidden {
    @include visually-hidden;
  }
  .portfolio_works-button_list {
    @include display;
    @include list;
    flex-wrap: wrap;
    margin-bottom: 40px;
  }
  .portfolio_works-button_box {
    margin-bottom: 15px;
    margin-right: 8px;
  }
  .portfolio_works-button {
    transition: box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1),
      background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
      color 250ms cubic-bezier(0.4, 0, 0.2, 1);
    padding: 6px 22px 6px 22px;
  
    &:hover {
      color: $core-color;
      background-color: $accent-color;
      box-shadow: 0px 3px 1px rgba(0, 0, 0, 0.1), 0px 1px 2px rgba(0, 0, 0, 0.08),
        0px 2px 2px rgba(0, 0, 0, 0.12);
      border-radius: 4px;
    }
    & {
      cursor: pointer;
      border: none;
      background: $background-ourteam-cl;
      border-radius: 4px;
      font-family: $font-main;
      text-align: center;
      font-size: 16px;
      font-weight: 500;
      line-height: 1.62;
      color: $main-text-color;
    }
  }
  .portfolio_works-flex_container {
    @include display;
    @include list;
    flex-wrap: wrap;
  }
  .portfolio_works-category_box {
    width: 100%;
    margin-bottom: 30px;
    transition: box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1);
  
    &:hover,
    &:focus {
      box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.12), 0px 4px 4px rgba(0, 0, 0, 0.06),
        1px 4px 6px rgba(0, 0, 0, 0.16);
    }
    &:hover .portfolio_works-title_box {
      transform: translateY(0);
    }
    & {
      background: $background-core-cl;
      border: 1px solid #eeeeee;
      box-sizing: border-box;
    }
  }
  .portfolio_works-flex_container .portfolio_works-category_box:nth-child(9) {
      margin-bottom: 0;
  }
  .portfolio_works-img_box {
    position: relative;
    overflow: hidden;
  }
  .portfolio_works-title_box {
    position: absolute;
    background-color: rgba(33, 150, 243, 0.9);
  
    & {
      position: absolute;
      left: 0;
      bottom: 0;
      height: 100%;
      margin: 0;
      padding: 63px 24px 0px 24px;
    }
    & {
      transform: translateY(100%);
      transition: transform 250ms cubic-bezier(0.4, 0, 0.2, 1);
    }
    & {
      font-family: $font-main;
      font-weight: normal;
      line-height: 1.56;
      color: $core-color;
    }

    @media screen and (min-width: 320px) {
      font-size: 14px;
    }
  }
  .portfolio_works-content_box {
    padding: 20px 24px 20px 24px;
  }
  .portfolio_works-content_title {
    margin: 0px 0px 5px 0px;
  
    & {
      font-family: $font-main;
      font-weight: bold;
      font-size: 18px;
      line-height: 2;
      letter-spacing: 0.06em;
      color: $main-text-color;
    }
  }
  .portfolio_works-content_style {
    margin: 0px;
  
    & {
      font-family: $font-main;
      font-weight: normal;
      font-size: 16px;
      line-height: 1.87;
      color: $second-color;
    }
  }
  
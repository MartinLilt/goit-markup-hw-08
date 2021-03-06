.backdrop {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.2);
  opacity: 1;
  transition: opacity 250ms cubic-bezier(0.4, 0, 0.2, 1);

  &.is-hidden {
    opacity: 0;
    pointer-events: none;
  }
  &.is-hidden .modal {
    transform: translate(-50%, -50%) scaleX(0.9);
  }
}
.modal {
  background-color: $core-color;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%) scaleX(1);
  transition: transform 250ms cubic-bezier(0.4, 0, 0.2, 1);

  & {
    box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.12), 0px 1px 1px rgba(0, 0, 0, 0.14),
      0px 2px 1px rgba(0, 0, 0, 0.2);
    border-radius: 4px;
  }

  @media screen and (min-width: 320px) {
    width: 290px;
  }

  @media screen and (min-width: 480px) {
    width: 450px;
  }
}
.modal-flex {
  @include display;
  padding-top: 8px;
}
.modal-social {
  cursor: pointer;
  @include display;
  padding: 10px;
  margin-left: auto;
  margin-right: 8px;
  border-radius: 50%;
  fill: $sup-color;
  border: 1px solid rgba(0, 0, 0, 0.1);
  transition: border 250ms cubic-bezier(0.4, 0, 0.2, 1),
    fill 250ms cubic-bezier(0.4, 0, 0.2, 1);

  &:hover {
    fill: $accent-color;
    border: 1px solid $accent-color;
  }
}
.modal-form_contentbox {
  padding: 0px 40px 40px 40px;
}
.modal-form_title {
  margin: 0px 0px 12px 0px;

  & {
    font-family: $font-main;
    font-weight: bold;
    font-size: 20px;
    line-height: 23px;
    text-align: center;
    color: $main-text-color;
  }
}
.modal-form_box {
  & .modal-form_field:nth-child(4) {
    margin-bottom: 20px;
  }
  & .modal-form_field:nth-child(5) {
    cursor: pointer;
    flex-direction: row;
    align-items: center;
    margin-bottom: 30px;
  }
}
.modal-form_field {
  position: relative;
  @include display;
  justify-content: flex-end;
  flex-direction: column;
  margin-bottom: 10px;

  & .modal-form_comm_input {
    resize: none;
    padding: 12px 16px 12px 16px;
  }
  & input[type="checkbox"] {
    @include visually-hidden;
  }
}
.modal-form_comm_input {
  &::placeholder {
    font-family: $font-main;
    font-weight: normal;
    font-size: 14px;
    line-height: 16px;
    letter-spacing: 0.01em;
    color: rgba(117, 117, 117, 0.5);
  }
  &:focus {
    outline: none;
    border: 1px solid $accent-color;
  }
  & {
    border: 1px solid rgba(33, 33, 33, 0.2);
    border-radius: 4px;
    min-height: 120px;
  }
}
.modal-form_label {
  margin-bottom: 4px;

  & {
    font-family: $font-main;
    font-weight: normal;
    font-size: 12px;
    line-height: 14px;
    letter-spacing: 0.01em;
    color: $second-color;
  }
}
.modal-form_input {
  padding-left: 42px;
  border: 1px solid rgba(33, 33, 33, 0.2);
  border-radius: 4px;
  height: 40px;

  &:focus {
    outline: none;
    border: 1px solid $accent-color;
  }
  &:focus ~ .modal-form_icon {
    fill: $accent-color;
  }
}
.modal-form_icon {
  position: absolute;
  top: 50%;
  left: 12px;

  & {
    fill: $main-text-color;
    overflow: hidden;
    transition: fill 250ms cubic-bezier(0.4, 0, 0.2, 1);
  }
}
.modal-form_icon:focus {
  fill: $accent-color;
}
.modal-checkbox_text {
  user-select: none;
  margin-left: 24px;

  & {
    font-family: $font-main;
    font-style: normal;
    font-weight: normal;
    font-size: 12px;
    line-height: 14px;
    letter-spacing: 0.03em;
    color: $second-color;
  }
  &_accent {
    text-decoration-line: underline;
    color: $accent-color;
  }
}
.modal-checkbox:checked ~ .modal-checkbox_icon {
  background-color: $accent-color;
  background-size: contain;
  background-origin: border-box;
  background-position: center;
  background-image: url(../images/icon-check.svg);
  border: $accent-color;
}
.modal-checkbox_icon {
  position: absolute;
  left: 0;
  top: 50%;
  transform: translateY(-50%);
  display: inline-block;
  border-radius: 2px;
  border: 2px solid $main-text-color;
  width: 16px;
  height: 15px;
}
.modal-form_button {
  @include auto-center;
  @include button-style;
  padding: 10px 55px 10px 55px;
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1);

  &:hover {
    background-color: $accent-hover-button;
  }
}

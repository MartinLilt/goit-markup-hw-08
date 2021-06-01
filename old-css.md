/* Website root #######################*/
:root {
  --accent-color: #2196f3;
  --main-text-color: #212121;
  --second-color: #757575;
  --core-color: #ffffff;
  --sup-color: #000000;
  --accent-color-button: #2196f3;
  --accent-hover-button: #188ce8;
  --background-core-cl: #ffffff;
  --background-ourteam-cl: #f5f4fa;
  --background-second-cl: #2f303a;
  --background-icon-team: #afb1b8;
  --border-color: #ececec;
  --font-logo: "Raleway", sans-serif;
  --font-main: "Roboto", sans-serif;
}

/* Website tag styles #######################*/
html {
  box-sizing: border-box;
}
*,
*::after,
*::before {
  box-sizing: inherit;
}

body {
  position: relative;
  font-family: "Raleway", sans-serif;
  font-family: "Roboto", sans-serif;
  font-style: normal;
  letter-spacing: 0.03em;
  background: var(--background-core-cl);
}

img {
  display: block;
  max-width: 100%;
  height: auto;
}
ul {
  list-style: none;
  padding: 0px;
}
a {
  text-decoration: none;
}

/* Website item styles #######################*/
.list {
  list-style: none;
}
.link-t {
  text-decoration: none;
}
.text-item {
  text-align: center;
}
.item-auto-center {
  margin-left: auto;
  margin-right: auto;
}
.mar-none {
  margin: 0px;
}
.padd-none {
  padding: 0px;
}
/* Website SVG icons #######################*/
.links-icon {
  margin-right: 10px;
  fill: currentColor;
}
.advantages-list-box::before {
  content: "";
  display: block;
  height: 120px;
  background-size: 70px;
  background-repeat: no-repeat;
  background-position: center;
  background-color: var(--background-ourteam-cl);
  margin-bottom: 30px;
}
.advantages-list-box:nth-child(1n)::before {
  background-image: url(../images/icons/icomoon/SVG/antenna.svg);
}
.advantages-list-box:nth-child(2n)::before {
  background-image: url(../images/icons/icomoon/SVG/clock.svg);
}
.advantages-list-box:nth-child(3n)::before {
  background-image: url(../images/icons/icomoon/SVG/diagram.svg);
}
.advantages-list-box:nth-child(4n)::before {
  background-image: url(../images/icons/icomoon/SVG/astronaut.svg);
}
.team-icon {
  fill: var(--background-icon-team);
}

/* Website containers #######################*/
.in-head-main-container {
  margin-left: auto;
  margin-right: auto;
  width: 1200px;
  padding-left: 15px;
  padding-right: 15px;
}
.main-container {
  margin-left: auto;
  margin-right: auto;
  width: 1200px;
  padding-left: 15px;
  padding-right: 15px;
}

/* Website position containers #######################*/
.advantages-position-container,
.img-list-position-container,
.portfolio-el-position-container,
.reg-customers-position-container {
  padding-bottom: 94px;
}

/* Website index/head menu #######################*/
.head-flex {
  display: flex;
  align-items: center;
}
.flex-nav {
  display: flex;
  padding: 32px 0px 32px 0px;
  margin: 0px;
}
.flex-nav .mr-li + .mr-li {
  margin-left: 50px;
}
.head-logo-position {
  margin-right: 93px;
}
.head-links-padd {
  padding-top: 32px;
  padding-bottom: 32px;
}
.head-contact-position {
  display: flex;
  margin-left: auto;
  padding: 0px;
}
.head-contact-position .mr-li + .mr-li {
  margin-left: 50px;
}
.contact-links-d {
  display: flex;
  align-items: center;
}
.nav-menu-d,
.contact-links-d {
  padding-top: 32px;
  padding-bottom: 32px;
  transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.nav-menu-d {
  position: relative;
}
.mr-li:nth-child(1) .nav-menu-d::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -1px;
  display: block;
  border-radius: 2px;
  width: 100%;
  height: 4px;
  background-color: var(--accent-color);
}
.mr-li:nth-child(1) .nav-menu-d {
  color: var(--accent-color);
}
.nav-menu-d:hover,
.nav-menu-d:focus,
.contact-links-d:hover,
.contact-links-d:focus,
.footer-contacts:hover,
.footer-contacts:focus {
  color: var(--accent-color);
}
.black-logo {
  font-family: var(--font-logo);
  font-weight: bold;
  font-size: 26px;
  line-height: 1.2;
  color: var(--main-text-color);
}
.blue-logo {
  color: var(--accent-color);
}
.nav-menu-d {
  font-family: var(--font-main);
  font-size: 14px;
  font-weight: 500;
  line-height: 1.14;
  letter-spacing: 0.02em;
  color: var(--main-text-color);
}
.contact-links-d {
  color: var(--second-color);
  font-family: var(--font-main);
  font-size: 14px;
  font-weight: 500;
  line-height: 1.14;
  letter-spacing: 0.02em;
}

/* Website index/core menu #######################*/
.backdrop {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.2);
  opacity: 1;
  transition: opacity 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.backdrop.is-hidden {
  opacity: 0;
  pointer-events: none;
}
.backdrop.is-hidden .modal {
  transform: translate(-50%, -50%) scaleX(0.9);
}
.modal {
  width: 528px;
  background-color: var(--core-color);
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%) scaleX(1);
  transition: transform 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.modal {
  box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.12), 0px 1px 1px rgba(0, 0, 0, 0.14),
    0px 2px 1px rgba(0, 0, 0, 0.2);
  border-radius: 4px;
}
.flex-modal {
  display: flex;
  padding-top: 8px;
}
.modal-social {
  cursor: pointer;
  display: flex;
  padding: 10px;
  margin-left: auto;
  margin-right: 8px;
  border-radius: 50%;
  fill: var(--sup-color);
  border: 1px solid rgba(0, 0, 0, 0.1);
}
.form-contentbox {
  padding: 0px 40px 40px 40px;
}
.form-title {
  margin: 0px 0px 12px 0px;
}
.form-title {
  font-family: var(--font-main);
  font-weight: bold;
  font-size: 20px;
  line-height: 23px;
  text-align: center;
  color: var(--main-text-color);
}
.form-field {
  position: relative;
  display: flex;
  flex-direction: column;
  margin-bottom: 10px;
}
.form .form-field:nth-child(4) {
  margin-bottom: 20px;
}
.form .form-field:nth-child(5) {
  cursor: pointer;
  flex-direction: row;
  align-items: center;
  margin-bottom: 30px;
}
.form-input {
  padding-left: 42px;
  border: 1px solid rgba(33, 33, 33, 0.2);
  border-radius: 4px;
  height: 40px;
}
.form-input:focus,
.form-comm-input:focus {
  outline: none;
  border: 1px solid var(--accent-color);
}
.form-input:focus ~ .form-icon {
  fill: var(--accent-color);
}
.form-label {
  font-family: var(--font-main);
  font-weight: normal;
  font-size: 12px;
  line-height: 14px;
  letter-spacing: 0.01em;
  color: var(--second-color);
}
.form-label {
  margin-bottom: 4px;
}
.form-icon {
  position: absolute;
  top: 50%;
  left: 12px;
}
.form-icon {
  fill: var(--main-text-color);
}
.form-comm-input {
  border: 1px solid rgba(33, 33, 33, 0.2);
  border-radius: 4px;
  min-height: 120px;
}
.form-field .form-comm-input {
  resize: none;
  padding: 12px 16px 12px 16px;
}
.form-comm-input::placeholder {
  font-family: var(--font-main);
  font-weight: normal;
  font-size: 14px;
  line-height: 16px;
  letter-spacing: 0.01em;
  color: rgba(117, 117, 117, 0.5);
}
.form-field input[type="checkbox"] {
  position: absolute !important;
  clip: rect(1px 1px 1px 1px);
  clip: rect(1px, 1px, 1px, 1px);
  padding: 0 !important;
  border: 0 !important;
  height: 1px !important;
  width: 1px !important;
  overflow: hidden;
}
.form-field {
  position: relative;
}
.checkbox-text {
  user-select: none;
  margin-left: 36px;
}
.checkbox-icon {
  position: absolute;
  left: 0;
  top: 50%;
  transform: translateY(-50%);
  display: inline-block;
  margin-left: 12px;
  border-radius: 2px;
  border: 2px solid var(--main-text-color);
  width: 16px;
  height: 15px;
}
.checkbox:checked ~ .checkbox-icon {
  background-color: var(--accent-color);
  background-size: contain;
  background-origin: border-box;
  background-position: center;
  background-image: url(../images/icon-check.svg);
  border: var(--accent-color);
}
.checkbox-text {
  font-family: var(--font-main);
  font-weight: normal;
  font-size: 14px;
  line-height: 1.71;
  color: var(--second-color);
}
.checkbox-text-accent {
  text-decoration-line: underline;
  color: var(--accent-color);
}
.form-button-text {
  padding: 10px 55px 10px 55px;
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.core-position-container {
  max-width: 1600px;
  margin-left: auto;
  margin-right: auto;
  background: var(--background-second-cl);
  padding-top: 200px;
  padding-bottom: 200px;
  background-image: linear-gradient(
      to right,
      rgba(47, 48, 58, 0.4),
      rgba(47, 48, 58, 0.4)
    ),
    url(../images/core-img.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}
.core-text {
  margin: 0px 0px 30px 0px;
}
.core-button-text {
  padding: 10px 32px 10px 32px;
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.core-button-text:hover,
.form-button-text:hover {
  background-color: var(--accent-hover-button);
}
.core-text {
  font-family: var(--font-main);
  font-weight: 900;
  font-size: 44px;
  line-height: 1.36;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--core-color);
}
.core-button {
  border: none;
  cursor: pointer;
  background: var(--accent-color-button);
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.15);
  border-radius: 4px;
  font-family: var(--font-main);
  font-weight: bold;
  font-size: 16px;
  line-height: 1.87;
  display: flex;
  align-items: center;
  letter-spacing: 0.06em;
  color: var(--core-color);
}

/* Website main/advantages list #######################*/
.advantages-position-container {
  padding-top: 94px;
}
.flex-container {
  display: flex;
  flex-wrap: wrap;
  padding: 0px;
}
.advantages-list-box {
  width: 270px;
  margin-right: 30px;
}
.advantages-list-box:nth-child(4n) {
  margin-right: 0px;
}
.h3-st {
  margin: 0px 0px 10px 0px;
}
.visually-hidden {
  position: absolute !important;
  clip: rect(1px 1px 1px 1px);
  clip: rect(1px, 1px, 1px, 1px);
  padding: 0 !important;
  border: 0 !important;
  height: 1px !important;
  width: 1px !important;
  overflow: hidden;
}
.list-title {
  font-family: var(--font-main);
  font-weight: bold;
  font-size: 14px;
  line-height: 1.14;
  text-transform: uppercase;
  color: var(--main-text-color);
}
.list-p {
  font-family: var(--font-main);
  font-weight: normal;
  font-size: 14px;
  line-height: 1.71;
  color: var(--second-color);
}

/* Website main/img list #######################*/
.h2-st {
  margin: 0px 0px 50px 0px;
}
.img-box:nth-child(3n) {
  margin-right: 0px;
}
.img-box {
  margin-right: 30px;
}
.img-pos-box {
  position: relative;
}
.img-title-box {
  position: absolute;
  width: 100%;
  left: 0;
  bottom: 0;
  background-color: rgba(47, 48, 58, 0.8);
  margin: 0px;
  padding-top: 27px;
  padding-bottom: 27px;
}
.What-are-we-doing {
  font-family: Roboto;
  font-weight: bold;
  font-size: 36px;
  line-height: 42px;
  color: var(--main-text-color);
}
.img-title-box {
  font-family: var(--font-main);
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;
  text-align: center;
  color: var(--core-color);
  text-transform: uppercase;
}
/* Website main/our team list #######################*/
.our-team-social-position {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.team-social-box {
  margin-right: 10px;
}
.team-social-box:nth-child(4n) {
  margin-right: 0px;
}
.our-team-social {
  display: flex;
  padding: 12px;
  border-radius: 50%;
  fill: var(--background-icon-team);
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
    fill 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.our-team-social:hover,
.our-team-social:focus {
  background-color: var(--accent-color);
  fill: var(--background-core-cl);
}
.our-team-svg {
  display: flex;
}
.bg-our-team {
  background: var(--background-ourteam-cl);
  padding-top: 94px;
  padding-bottom: 94px;
}
.h2-st2 {
  margin: 0px 0px 50px 0px;
}
.advantages-list-box-4 {
  margin-right: 30px;
}
.advantages-list-box-4:nth-child(4n) {
  margin-right: 0px;
}
.our-team-title {
  margin: 0px 0px 10px 0px;
}
.our-team-p {
  margin: 0px 0px 16px 0px;
}
.our-team-title-box {
  padding: 30px 32px 30px 32px;
}
.our-team {
  font-family: var(--font-main);
  font-weight: bold;
  font-size: 36px;
  line-height: 1.17;
  color: var(--main-text-color);
}
.our-team-title {
  font-family: var(--font-main);
  font-size: 16px;
  font-weight: 500;
  line-height: 1.19;
  color: var(--main-text-color);
}
.our-team-p {
  font-family: var(--font-main);
  font-weight: normal;
  font-size: 16px;
  line-height: 1.19;
  color: var(--second-color);
}
.our-team-box {
  background: var(--background-core-cl);
  box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.12), 0px 1px 1px rgba(0, 0, 0, 0.14),
    0px 2px 1px rgba(0, 0, 0, 0.2);
  border-radius: 0px 0px 4px 4px;
}
/* Website regular customers #######################*/
.reg-customers-position-container {
  padding-top: 94px;
}
.reg-customers-flex {
  display: flex;
  flex-wrap: nowrap;
  align-items: center;
}
.reg-customers-box {
  margin-right: 30px;
}
.reg-customers-box:nth-child(6n) {
  margin-right: 0px;
}
.reg-customers-svg {
  display: flex;
}
.reg-customers-social {
  display: flex;
  padding: 15px 31px 15px 31px;
  border-radius: 4px;
  border: 1px solid var(--background-icon-team);
  fill: var(--background-icon-team);
  transition: border 250ms cubic-bezier(0.4, 0, 0.2, 1),
    fill 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.reg-customers-social:hover,
.reg-customers-social:focus {
  fill: var(--accent-color);
  border: 1px solid var(--accent-color);
}
/* Website footer #######################*/
.footer-social {
  display: flex;
  padding: 12px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.1);
  fill: var(--core-color);
}
.footer-social {
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
    fill 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.footer-social:hover,
.footer-social:focus {
  background-color: var(--accent-color);
  fill: var(--background-core-cl);
}
.footer-svg {
  display: flex;
}
.footer-flex {
  display: flex;
}
.footer-addres {
  margin-right: 70px;
}
.footer-links {
  margin-right: 93px;
}
.footer-lead {
  min-width: 570px;
}
.footer-button-svg {
  display: flex;
  margin-left: 11px;
  fill: var(--core-color);
}
.footer-button-text {
  padding: 10px 28px 10px 28px;
  transition: background-color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.footer-button-text:hover {
  background-color: var(--accent-hover-button);
}
.footer-button {
  border: none;
  cursor: pointer;
  background: var(--accent-color-button);
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.15);
  border-radius: 4px;
  font-family: var(--font-main);
  font-weight: bold;
  font-size: 16px;
  line-height: 1.87;
  display: flex;
  align-items: center;
  letter-spacing: 0.06em;
  color: var(--core-color);
}
.footer-form {
  display: flex;
  align-items: center;
}
.footer-field {
  display: flex;
  margin-right: 12px;
}
.bg-footer-container {
  padding-bottom: 60px;
  padding-top: 60px;
  background: var(--background-second-cl);
}
.footer-container {
  margin-left: auto;
  margin-right: auto;
  width: 1170px;
}
.footer-logo-pos {
  margin-bottom: 20px;
  display: block;
}
.footer-address-pos {
  margin-bottom: 10px;
  display: block;
}
.footer-links-pos {
  margin-bottom: 10px;
  display: block;
}
.footer-logo {
  color: var(--accent-color);
}
.footer-customers-p {
  margin: 12px 0px 20px 0px;
}
.footer-contacts {
  transition: color 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.footer-customers-p {
  font-family: var(--font-main);
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;
  text-transform: uppercase;
  color: var(--core-color);
}
.footer-logo-white {
  font-family: var(--font-logo);
  font-weight: bold;
  font-size: 26px;
  line-height: 1.19;
  color: var(--core-color);
}
.address {
  font-style: inherit;
  font-family: var(--font-main);
  font-weight: normal;
  font-size: 14px;
  line-height: 1.71;
  letter-spacing: 0.03em;
  color: var(--core-color);
}
.footer-contacts {
  font-family: var(--font-main);
  font-weight: normal;
  font-size: 14px;
  line-height: 1.71;
  color: rgba(255, 255, 255, 0.6);
}
.footer-input {
  padding-left: 16px;
  height: 50px;
  min-width: 358px;
  outline: none;
}
.footer-input:focus {
  border: 1px solid var(--accent-color);
}
.footer-input::placeholder {
  font-family: var(--accent-color);
  font-weight: normal;
  font-size: 16px;
  line-height: 1.25;
  color: rgba(255, 255, 255, 0.6);
}
.footer-input {
  background-color: rgba(0, 0, 0, 0);
  border: 1px solid rgba(255, 255, 255, 0.3);
  filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.15));
  border-radius: 4px;
}
/* Website portfolio page header #######################*/
.portfolio-head-position-container {
  border: 1px solid var(--border-color);
}
.flex-nav .portfolio-mr-li + .portfolio-mr-li {
  margin-left: 50px;
}
.head-contact-position .portfolio-mr-li + .portfolio-mr-li {
  margin-left: 50px;
}
.portfolio-mr-li:nth-child(2) .nav-menu-d::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -1px;
  display: block;
  border-radius: 2px;
  width: 100%;
  height: 4px;
  background-color: var(--accent-color);
}
.portfolio-mr-li:nth-child(2) .nav-menu-d {
  color: var(--accent-color);
}
/* Website portfolio page buttons #######################*/
.portfolio-el-position-container {
  padding-top: 94px;
}
.portfolio-btn-position-container {
  margin-bottom: 50px;
}
.portfolio-buttons-list {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
.btn-li {
  margin-right: 8px;
}
.btn-li:nth-child(5n) {
  margin-right: 0px;
}
.btn {
  transition: box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1),
    background-color 250ms cubic-bezier(0.4, 0, 0.2, 1),
    color 250ms cubic-bezier(0.4, 0, 0.2, 1);
  padding: 6px 22px 6px 22px;
}
.btn:hover {
  color: var(--core-color);
  background-color: var(--accent-color);
  box-shadow: 0px 3px 1px rgba(0, 0, 0, 0.1), 0px 1px 2px rgba(0, 0, 0, 0.08),
    0px 2px 2px rgba(0, 0, 0, 0.12);
  border-radius: 4px;
}
.btn {
  cursor: pointer;
  border: none;
  background: var(--background-ourteam-cl);
  border-radius: 4px;
  font-family: var(--font-main);
  text-align: center;
  font-size: 16px;
  font-weight: 500;
  line-height: 1.62;
  color: var(--main-text-color);
}

/* Website portfolio page categories #######################*/
.portfolio-main-flex {
  display: flex;
  flex-wrap: wrap;
}
.port-bc {
  width: 370px;
  margin-right: 30px;
  margin-bottom: 30px;
  transition: box-shadow 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.portfolio-img-box {
  position: relative;
  overflow: hidden;
}
.portfolio-img-title-box {
  position: absolute;
  background-color: rgba(33, 150, 243, 0.9);
}
.port-bc:hover,
.port-bc:focus {
  box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.12), 0px 4px 4px rgba(0, 0, 0, 0.06),
    1px 4px 6px rgba(0, 0, 0, 0.16);
}
.port-bc:nth-child(3n) {
  margin-right: 0px;
}
.port-bc:nth-last-child(-n + 3) {
  margin-bottom: 0px;
}
.port-title {
  margin: 0px 0px 5px 0px;
}
.port-p {
  margin: 0px;
}
.port-title-box {
  padding: 20px 24px 20px 24px;
}
.portfolio-img-title-box {
  position: absolute;
  left: 0;
  bottom: 0;
  height: 100%;
  margin: 0;
  padding: 63px 24px 0px 24px;
}
.portfolio-img-title-box {
  transform: translateY(100%);
  transition: transform 250ms cubic-bezier(0.4, 0, 0.2, 1);
}
.port-bc:hover .portfolio-img-title-box {
  transform: translateY(0);
}
.portfolio-img-title-box {
  font-family: var(--font-main);
  font-weight: normal;
  font-size: 18px;
  line-height: 1.56;
  color: var(--core-color);
}
.port-title {
  font-family: var(--font-main);
  font-weight: bold;
  font-size: 18px;
  line-height: 2;
  letter-spacing: 0.06em;
  color: var(--main-text-color);
}
.port-p {
  font-family: var(--font-main);
  font-weight: normal;
  font-size: 16px;
  line-height: 1.87;
  color: var(--second-color);
}
.port-bc {
  background: var(--background-core-cl);
  border: 1px solid #eeeeee;
  box-sizing: border-box;
}

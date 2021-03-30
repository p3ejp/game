


class Fish {
  constructor() {
    this.x = 50;
    this.y = height - 50;
    this.vy = 0;
    this.gravity = 0.5;
  }

  jump() {
    this.vy = -5;
  }

  move() {
    this.y += this.vy;
    this.vy += this.gravity;
    this.y = constrain(this.y, 0, height - 50);

  }

  show() {

    image(fimg, this.x, this.y + -70, 100, 120);
  }

}


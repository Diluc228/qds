from random import*
shar = ("", 200, 250,40,40)
dx = -2
dy = -2
speedx = 3
speedy = 3
while game:
    for i in event.get():
        if i.type==QUIT:
            game - False
    shar.ris()
    shar.rect.x = shar.rect.x +speedx*dx
    shar.rect.y = shar.rect.y +speedy*dy
    if shar.rect.x <= 0:
        dx *= -1
        speedx = randint(3,5)
        speedy = randint(3,5)
    if shar.rect.x > 470:
        dx *= -1
        speedx = randint(3,5)
        speedy = randint(3,5)
    if shar.rect.y <= 0:
        dy *= -1
        speedx = randint(3,5)
        speedy = randint(3,5)
    if shar.rect.y > 470:
        dy *= -1
        speedx = randint(3,5)
        speedy = randint(3,5)
    display.update()
    clock.tick(40)

# DanceBattle - Cupid

 def _gopigo3_command_dance(self):
        print("DANCE OFF!")
        b = 60/120
        x = 1
        
        while x <= 1:
            #START
            print("1st")
            self.gopigo3.open_eyes()
            self.left_eye_on = self.right_eye_on = True
            self.gopigo3.right()
            sleep(2*b)
            self.gopigo3.forward()
            sleep(2*b)
            self.gopigo3.left()
            sleep(2*b)
            self.gopigo3.forward()
            sleep(2*b)
            self.gopigo3.right()
            sleep(16*b)
        
            #U TURN
            print("2nd")
            self.gopigo3.steer(100, 20)
            end_speed = 2000
            self.gopigo3.set_speed(end_speed)
            sleep(8*b)

            #FREESTYLE
            print("3rd")
            self.gopigo3.stop()
            print("left")
            self.gopigo3.left()
            sleep(4*b)
            print("back")
            self.gopigo3.backward()
            sleep(2*b)
            print("forward")
            self.gopigo3.forward()
            sleep(2*b)
            print("right")
            self.gopigo3.right()
            sleep(10*b)
            
            x = x + 1
            self.gopigo3.stop()
            sleep(4*b)
        
        while x == 2:
            print("4th")
            self.gopigo3.forward()
            sleep(0.75*b)
            self.gopigo3.stop()
            sleep(0.5*b)
            x = x + 1
            
        while x == 3:
            self.gopigo3.close_eyes()
            self.left_eye_on = self.right_eye_on = False
            self.gopigo3.forward()
            sleep(4*b)
            self.gopigo3.stop()
            x = x + 1
            
        while x == 4:
            sleep(5.75*b)
            self.gopigo3.open_eyes()
            self.left_eye_on = self.right_eye_on = True
            sleep(0.25*b)
            self.gopigo3.stop()
            sleep(2*b)
            self.gopigo3.forward()
            x = x + 1
        
        while x == 5:
            print("1st")
            self.gopigo3.right()
            sleep(2*b)
            self.gopigo3.forward()
            sleep(2*b)
            self.gopigo3.left()
            sleep(2*b)
            self.gopigo3.forward()
            sleep(2*b)
            self.gopigo3.right()
            sleep(16*b)
            x = x + 1
            
        while x == 6:
            self.gopigo3.stop()
            x = x + 1

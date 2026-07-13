
mm/dd/yy format

# Day 1 (7/9/26): Starting out (time spent 3 hours)

Brainstormed some ideas for how a ball launcher robot would like and function. I compared different designs on exisitng robots as well and settled on a 2 dof shooter with a turret like design. Additionally, there will be 2 flywheels for front / backspin. 

<img width="546" height="444" alt="Screenshot 2026-07-09 at 6 05 33 PM" src="https://github.com/user-attachments/assets/6fcc190c-d175-41c6-8d08-23681e04618a" />

I was also looking for parts and i've roughly decided what I'm planning on using:
- 2x dc motors for the flywheels
- 2x servos for turret control
- esp32 for the brain of the system
- 3d printed shell
- tube for the ping pong balls
- either custom or off the shelf motor controllers
- 8x AA battery for power source

# Day 2 (7/10/26): Designing the build + more ideas (time spent 2 hours)

I was thinking that the robot should also be able to place the ball according to how the opponent is playing so it should be connected to a camera which can detect the play location and hit the ball opposite to the player location. Additionally, it should know when the ball has been hit to its side of the court.

<img width="430" height="504" alt="Screenshot 2026-07-11 at 6 16 27 PM" src="https://github.com/user-attachments/assets/b8585bb3-6581-497b-ab48-ca7b04078698" />


# Day 3 (7/11/26): Cad Progress (time spent 5 hours)

Today was mostly working on the cad for the ball launcher. I fully developed the launcher module with 2 flywheels along with the pivot structure.

<img width="426" height="471" alt="Screenshot 2026-07-11 at 11 57 07 PM" src="https://github.com/user-attachments/assets/8bb8846f-137e-442d-894a-393a17de3b48" />

This is the shooter and the gaps are where the flywheels sit.

This is the pivot platform which will rotate left to right allowing for the ball to be shot to different locations. Additionally, the pullars on the side will be mounting points for the shooter, allowing it to rotate up and down for differnt angled shots.

<img width="230" height="281" alt="Screenshot 2026-07-11 at 11 58 00 PM" src="https://github.com/user-attachments/assets/1fd9b237-a997-47c1-b95e-4a20206b60fc" />

This is all the pieces put together.

<img width="459" height="473" alt="Screenshot 2026-07-11 at 11 59 52 PM" src="https://github.com/user-attachments/assets/ebe94f55-963d-4cca-8252-36edca1c2b15" />

The next steps are to figure out a feeding system for the shooter to allow for balls to be shot one by one and a platform for the pivot plate to sit on so a servo can fit underneath

# Day 4 (7/12/26): Final Design (time spent 5 hours)

Today I finished up the cad for the robot. The design was changed a little bit so now the hopped is directly integrated instead of it being a tube that feeds. Additionally, I made a rotation stand for the base so the servo is more stable along with a change in servo placement for the tilt so that it is more compact.

<img width="439" height="434" alt="Screenshot 2026-07-12 at 11 20 43 PM" src="https://github.com/user-attachments/assets/fe54c656-4392-452f-99f6-4fead4897994" />

Shooter and hopper. This design allows for a controlled release of balls.

<img width="408" height="150" alt="Screenshot 2026-07-12 at 11 21 57 PM" src="https://github.com/user-attachments/assets/e78b6a9f-cec9-4740-8a9b-3dac9962426b" />

This is the base plate with the servo

<img width="338" height="460" alt="Screenshot 2026-07-12 at 11 25 25 PM" src="https://github.com/user-attachments/assets/8ea3a292-8e22-48ba-ac07-a273904d4c22" />

Final design, the hopper is very light and design to counteract the torque of the 2 motors, making it easier for the servo to tilt the structure

Here is the final bom:

- 2x [DC motor 12V](https://www.amazon.com/AUTOTOOLHOME-Torque-Traxxas-Wheels-Electric/dp/B01M58POHF/ref=pd_ci_mcx_di_int_sccai_cn_d_sccl_1_1/142-3738919-8988922?pd_rd_w=cI11X&content-id=amzn1.sym.751acc83-5c05-42d0-a15e-303622651e1e&pf_rd_p=751acc83-5c05-42d0-a15e-303622651e1e&pf_rd_r=KS914ZRRX66DD1SZYE5D&pd_rd_wg=xGBrP&pd_rd_r=d860e736-02ab-4be9-9de8-45b8fbe8bdae&pd_rd_i=B01M58POHF&psc=1) $13.78
- 4x [high 55g torque servos](https://www.amazon.com/Hosyond-MG996R-Digital-Motors-Helicopter/dp/B0BYD9M1P3/ref=pd_lpo_d_sccl_1/142-3738919-8988922?pd_rd_w=GY3yi&content-id=amzn1.sym.4c8c52db-06f8-4e42-8e56-912796f2ea6c&pf_rd_p=4c8c52db-06f8-4e42-8e56-912796f2ea6c&pf_rd_r=NA9N97EKKA1KCF0VZVCP&pd_rd_wg=eLkzT&pd_rd_r=88d0f238-0f73-45bd-8654-424eb752af9b&pd_rd_i=B0BYD9M1P3&th=1) $17.99
- 3x [esp32 devkit c v4](https://www.amazon.com/ESP32-DevKitC-32-Development-Supporting-Bluetooth-Interface/dp/B0DYDN5X1Z/ref=sr_1_11?crid=2DXP1KTKVEXMB&dib=eyJ2IjoiMSJ9.OxudVGZzwAljFhIXZMie6Nnr8FwdUEAeOxlJae2ITRBaLrNGPMIyCTf0e7cUAFXuPq0Mn7a0p7bpzz8c_f-UNgeFK1FM3cfe3FV2aFIXWnepVTECsvkHdpBfeStJxTpgtghA9WOWYI19rOhfxa8LWiW2F99n166f7Zp5-L2TXt8KwA26h1cmrngWDSoLlpaTMeM_7qUQ4JMvtkUYLDCi95cT7o-ng2qcMwGp93om2yY.o1TsEeZ6HNjEl-4MyaGxEqTIKg1abF1aayn9t6hDf9o&dib_tag=se&keywords=esp32+usb+c+38+pin&qid=1783924563&sprefix=esp32+usb+c+38+pi%2Caps%2C186&sr=8-11) $17.99

Total: $49.76






# LinkedIn kit

## Main post (post natively with the video; ~1,300 chars)
11.6 mm to 5 mm.

That's how far I had to shrink my robot's pen error before it could write Kannada cleanly.

This Diwali I built a MuJoCo simulation where a UR5e cobot:

🪔 writes ಎಲ್ಲರಿಗೂ ದೀಪಾವಳಿ ಹಬ್ಬದ ಶುಭಾಶಯಗಳು on a board
🪔 adds a small HAPPY DIWALI underneath
🪔 lights a rocket's fuse at the bottom, the way you'd do it for real
🪔 then the rocket launches and blasts across the sky

Kannada was the hard part. The letters curve, stack and join, so I pulled the glyph outlines from a font and turned them into pen strokes the arm follows with inverse kinematics. The default controller gains missed the line by 11.6 mm. Stiffer joint gains plus feedforward got it to about 5 mm, and the script became readable.

It runs fully offline on a MacBook, with a live speed control from 0.2x to 3x. The robot model is the open-source UR5e from MuJoCo Menagerie.

Simulation is where I test ideas before a real arm ever moves. Festivals just make the testing more fun.

Happy Diwali to everyone in my network 🪔

Which language would you want a robot to write your greeting in?

P.S. Setup notes are in the first comment.

#Robotics #MuJoCo #Diwali

## First comment (post right after)
Setup notes for anyone who wants to try it:

• Robot: UR5e from MuJoCo Menagerie (open source)
• Install: pip install mujoco, then run with mjpython on macOS
• Controls: UP/DOWN = speed, SPACE = pause, R = replay, C = camera

Code: <ADD YOUR GITHUB REPO LINK>

If you try it, tell me what greeting you made it write.

## Short version
A robot arm wrote "ಎಲ್ಲರಿಗೂ ದೀಪಾವಳಿ ಹಬ್ಬದ ಶುಭಾಶಯಗಳು" in Kannada, then lit a rocket fuse at the bottom and launched it.

All in simulation, on my MacBook, offline.

UR5e cobot + MuJoCo + one very stubborn weekend of getting the pen error from 11.6 mm down to 5 mm.

Happy Diwali from Bengaluru 🪔

What should I teach it to write next?

#Robotics #Diwali #MuJoCo

## Reach checklist
- Upload the video natively (not a YouTube/Drive link); keep it under ~60 s (`--speed 1.3`)
- Use `images/linkedin_cover_1200x627.png` as a second image or the video thumbnail
- Post Tue/Wed/Thu, 7:30-9:00 AM IST; link in the FIRST COMMENT, not the body
- Reply to every comment in the first hour; ask 5-10 robotics friends to comment genuinely
- Comment on 5-10 other robotics/Diwali posts before and after you post
- Keep to 3 hashtags; no "comment X to get Y" bait

## Follow-up post ideas (week 2)
1. "How I turned a font into robot pen strokes" (Kannada glyph to IK pipeline)
2. "Why default UR5e gains miss by 11.6 mm" (controller tuning)
3. Behind-the-scenes screen recording of the speed control

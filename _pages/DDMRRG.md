---
permalink: /DDMRRG/
title: "Data-driven Model Reduction Reading Group"
author_profile: false
---


<iframe src="https://calendar.google.com/calendar/embed?height=600&wkst=1&bgcolor=%23ffffff&ctz=America%2FPhoenix&mode=AGENDA&src=Y18xYXJkNHFnMTkxazBwdGx0OXVqcGFrNjBvZ0Bncm91cC5jYWxlbmRhci5nb29nbGUuY29t&color=%23AD1457" style="border:solid 1px #777" width="700" height="400" frameborder="0" scrolling="no"></iframe>


Nov 23, 2021
====

Today Alexa walked us through her research topic and how model reduction relates to her goals. 


Nov 16, 2021
====
Today I (Jared McBride) continued the discussion of Dr. Lin's [paper](/files/DDMRRG/LinLu20.pdf) and the type of model reduction I am interested in. Particularly, we discussed in greater detail the user-chosen ansatz and how Dr. Lin handled certain stability issues in the implementation presented in the paper. We then discussed how a natural relation between numerical Wiener filtering and least squares problems, allows for simpler solutions. However, we observed that these simpler solutions may have stabilities issues.  

As far as other least squares solvers, we also discussed a randomizer least squares solver due to Kaczmarz. It has been extended by A. Zouzias and N. M. Freris, who wrote [this paper](/files/DDMRRG/Kaczmarz.pdf).

Here are the [notes](/files/DDMRRG/DDMRRG-Nov16.html) (continued from Nov 9) and here is the meeting [recording](https://arizona.zoom.us/rec/share/eGLKja3tyTW-fjZSjJNIqB8efJ1n3SmIGsv_d4JdbYce6lIMuzGU8gTFwydk6ck8.L6J7Yseis2wbTusE?startTime=1637075113000).



Nov 9, 2021
====
Today I (Jared McBride) took us through the first 3 sections of Dr. Lin's [paper](/files/DDMRRG/LinLu20.pdf)

Here are the [notes](/files/DDMRRG/DDMRRG-Nov9.html) and here is the meeting [recording](https://arizona.zoom.us/rec/share/dw1Nxz8Fs0AJqVLLe3I9MWgDTNfaENt2F12_y53JyFcVl031dlquE71T_KFzg65J.AR05AiUU_ooqifZl?startTime=1636470325000).



Nov 2, 2021
====
In our meeting today we looked at a tutorial on DMD, which can be found at [this site](https://mathlab.github.io/PyDMD/tutorial1dmd.html). At first it did not make sense to me why $f_1$ and $f_2$ were dynamic modes. So, we discussed this a little as we looked through the tutorial.

Here's a little information on that:

So, we have

$$
\begin{align*}
f_1(x,t)&=\text{sech}(x+3)\exp(i2.3t)\\
f_2(x,t)&=2\text{sech}(x)\tanh(x)\exp(i2.8t)
\end{align*}
$$

And our data is the sum of these two functions evaluated on the unifomrly spaced grid with $-5\le x_j \le 5$ (128 points) and $0 \le t_i \le 4\pi$ (256 points). So, using the following notation
- $f = f_1 + f_2$
- $\mathbf{x} = \text{col}(x_j, ~~ j = 1,\dots, 128)$
- $X_n = f(\mathbf{x},t_n) = \text{col}(f(x_j,t_n), ~~ j = 1,\dots, 128)$

I think of some map $F$ such that

$$
F(X_n) = X_{n+1}
$$

and DMD as finding the eigenvalues and eigenfunctions of a liner least squares approximation of $F$, namely $A$. It was not clear to me how $f_1(\mathbf{x},\cdot)$ or $f_2(\mathbf{x},\cdot)$ could be or approximate the eigenfunctions of $A$. But then I considered the following

$$
F(f_1(\mathbf{x},t_n)) \approx f_1(\mathbf{x},t_{n+1}) = f_1(\mathbf{x},t_{n})e^{i2.3*\Delta t}
$$


Then we looked at DMD being applied to numerical solutions to the Kuromoto-Sivashinsky equation (it did not do well).  

There are two recordings this time because I accidentaly closed the meeting trying to get the ipad to annotate. Here are the links
- [First half](https://arizona.zoom.us/rec/share/dxh5jpP5MGfglO3gE--CclDwYmsBVmePrLefMSdCS0qurd-t1lHmrnJhkvvWqACh.KM_Vy1RjYI2hKUsD)
- [Second Half](https://arizona.zoom.us/rec/share/GcAdgoSg7hqNRArnrPKKWuX8IeYOx_oiOsVpgM3ek5WTGZVf3CFHUn9MbUqZuU31.kpkkD_N9jN7IuiX2)

Next meeting (Nov 9) I will be presenting the sort of data-driven modeling I do. In preparation I recomened we look over [this paper by Dr. Lin](/files/DDMRRG/LinLu20.pdf).

Oct 28, 2021
====
In are meeting on Tuesday (Oct 26) we dicsussed more from the first reference below ([Data-driven methods for reduced-order modeling](/files/DDMRRG/Data-Driven_methods_for_reduced-order_modeling--Kutz+Brunton.pdf)). The meeting can be viewed [here](https://arizona.zoom.us/rec/share/EGfcYgofOfdoBHRPFcW3wbG2gL199x2cOlYL-DNNboBva-62q-ap03G0pCVaRXiV.aQK5XVS_Cgv64ZpL?startTime=1635260472000). Our discussion focused on DMD and a little into the Koopman operator. I think an example would be really nice so I and maybe Micheal will try to have one next meeting.

For next meeting the plan is to continue with the current paper hopefully getting to SINDy and beyond, perhaps looking at the Klus reference,  [Data-Driven Model Reduction and Transfer Operator Approximation](/files/DDMRRG/Data-Driven_Model_Reduction_and_Transfer_Operator--Klus2018.pdf).



Oct 22, 2021
====
[Here](https://www.youtube.com/watch?v=sQvrK8AGCAo) is a video of Steven Brunton explaining DMD. I found it very enlightening, and it is less than twenty minutes.  


Oct 19, 2021
====
Today we went over the first reference below ([Data-driven methods for reduced-order modeling](/files/DDMRRG/Data-Driven_methods_for_reduced-order_modeling--Kutz+Brunton.pdf)). The meeting can be viewed [here](https://arizona.zoom.us/rec/share/hRSBoQMZ8N-vlmNzBRx9yiS1YGqYqSEKMu9-wlnDxJPMlOE-qz0XSSG7jkbfrNBh.3UlYgIZ2cMNiss7D) We talked a lot about SVD and a little about DMD (dynamic mode decomposition). We decided to push back mine and Alexa's presentation by a week so that we can talk more about this reference next week. The plan will be to finish our discussion of the work and then the week after discuss Klus' paper.


Oct 18, 2021
====
Per our discussion last week we have decided to move times in order to accommodate more people. The new time of the meetings is 8 AM. I have changed the room to ENR2 S375 (that is the small conference room that shares a wall with the kitchen) since there are not a ton of us and I think that room has some technology that may facilitate our zoom meetings.

So, we decided to kick off our meetings with a crash course in data-driven model reduction and there are a few good references that I have seen for this.

* [Data-driven methods for reduced-order modeling](/files/DDMRRG/Data-Driven_methods_for_reduced-order_modeling--Kutz+Brunton.pdf) by Brunton and Kutz is a textbook chapter. It introduces dynamic model decomposition (DMD) and Koopman theory. It also has a section on data-driven model discovery which includes SINDy.
* [Data-Driven Model Reduction and Transfer Operator Approximation](/files/DDMRRG/Data-Driven_Model_Reduction_and_Transfer_Operator--Klus2018.pdf) by Stefan Klus et al. is a journal article and goes over a number of techniques and applications. DMD is a significant part of it.
* [Galerkin v. least-squares Petrov–Galerkin projection in nonlinear model reduction](/files/DDMRRG/Galerkin_v_least-squares_Petrov–Galerkin_projection_in_NL_MR--Carlsberg+Barone+Antil.pdf)  by Carlberg et al. has a description of Galerkin ROM. I think it may be useful if you have not seen Galerkin's method before, since the first two papers assume knowledge of it.
* [Introduction to Model Order Reduction](/files/DDMRRG/Introduction_To_Model_Order_Reduct--Schilders.pdf) by Wil Schilders may be useful too, it seems to briefly explain quite a few methods.

For tomorrow, let's read as much as we are able from the first reference (Brunton and Kutz, both of which have lectures on Youtube in reduced order modeling) and then discuss it.


Oct 12, 2021
====
Today we had an organizational meeting and it was decided that the group would be a mix between a journal club and a seminar (a more informal seminar). Next week we will be go over a survey. So, we will all look for a good survey of various forms of data-driven model reduction and the best one we find by Thursday will be sent out to the group.

The meeting can be viewed [here](https://arizona.zoom.us/rec/share/YlbbP16vK0-d_b7EFn-JYEo-jzPbpiYorUBj9MIQb27M79_-Z6HeROalEw2oTrUJ.SijL1L2rkkpH5fCo). Apologies for the poor sound quality, I will investigate getting a better webcam with microphone.

We also made up a schedule with a calendar (now permenatly displayed above.)


Oct 11, 2021
====
Because of poor attendance at last week's meeting, I thought we would try again at the organizational meeting. So, let's meet tomorrow at 2:00 PM in room Math 402. I will be hosting a Zoom meeting too, if you would prefer
to meet electronically. The zoom link is [https://arizona.zoom.us/s/9826305419](https://arizona.zoom.us/s/9826305419)

Having spoken to a few members of the group throughout the week. I think a strong benefit to the group could come from those doing DDMR research to share what they are doing through a short informal talk. Many of us do fairly different forms of DDMR. and these talks would allow for a sort of cross-pollination of ideas. These talks would be different from a seminar talk in that there would be much more open dialogue as we discuss more in depth the issues and fixes found in each person's own flavor of DDMR. That being said, I am prepared to give such a talk on the 19th (next week), should we decide tomorrow to try this proposed format. I can also send some references that demonstrate this type of model reduction.

Anyway, as always if you have any Ideas, please feel free to email me.



Sept 28, 2021
====
The first meeting will be in the math building room 402 and on Zoom at this Zoom [link](https://arizona.zoom.us/s/9826305419), on **Tuesday, October 5 at 2:00 PM**. This will be an organizational meeting.


Sept 27, 2021
====

Welcome to the Data-driven Model Reduction Reading Group page. Here is will I will post articles, talk slides and links to Zoom meeting recordings.

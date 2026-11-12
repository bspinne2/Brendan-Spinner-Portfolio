# Lab 11) Snap Fit Design for SLA Printing

<img width="1465" height="597" alt="Screenshot 2026-11-12 144440" src="https://github.com/user-attachments/assets/d9d682db-de21-43e2-91b1-c46e24122937" />

This assignment requires me to go back to what I learned to do last week, utilizing a SLA resin printer, alcohol bath and curator to create a finished print that is functional and higher quality than a standard filament print. However for this assignment, I am focused on creating a snap-fit design rather than a sliding fit.

## Research & Modeling Principles

For my 35mm by 35mm by 20mm box (1.2mm walls), I chose a straight rectangular cantilever snap-fit because it allows the latch arm (4.0mm long & wide) to flex elastically during assembly and snap back into an unstressed resting state. To keep the arm from snapping under stress, I planned to add a 0.6mm root fillet at the base and used a 30 degree lead-in angle and a 45 degree push-out angle so the lid is easy to close but still removable. I also included a 0.2mm clearance across the lid lip and retaining slot (4.2mm wide) so the parts fit together cleanly after printing.

A cantilever snap-fit is governed by the relationship between deflection (y), beam thickness (h), and beam length (L), where maximum strain is equal to (3yh/2L^2). Keeping the undercut small (0.6mm) prevents the outer fibers of the beam from exceeding the material's strain limit. Assembly force depends directly on the lead-in angle and friction, which is why matching the 30 degree hook angle with a 30 degree chamfer on the lid slot lowers insertion force, while the steeper 45 degree return angle holds the lid shut. Finally, beam stiffness scales with the cube of thickness (h^3) and width (b = 4.0mm), giving the latch enough rigidity to hold the lid securely without twisting.

Because Form 4 SLA resins are cross-linked thermosets, they are much stiffer and more brittle than standard injection-molded plastics like polypropylene. This makes it ever so crucial to eliminate any sharp corners or excessive force that could break the print when the fit goes through deformation.

## Snap-Fit CAD Design

I drew inspiration for this simple snap fit design from something I saw on printables.com. I wanted to satisfy the assignment criteria while also keeping the overall design simplistic and non-complicated. 

<img width="1821" height="927" alt="Screenshot 2026-11-10 091123" src="https://github.com/user-attachments/assets/61c0f436-4940-4c27-98f9-661e740b8296" />

<img width="811" height="597" alt="Screenshot 2026-11-10 091156" src="https://github.com/user-attachments/assets/d17a2ae6-9f83-4441-b19b-5de09a371d24" />

The inspiration print implements a singular latch that bends and snaps into a mating hole on the lid part. This sort of build while unoriginal, is very versatile in its usability and can be used for a multitude of different purposes.

I began the build by parametrically modeling with some dimensions that Gemini AI suggested would be smart for a build like mine.

<img width="767" height="248" alt="Screenshot 2026-11-10 092138" src="https://github.com/user-attachments/assets/a22cfea0-1090-47ea-8cb4-0dfe68af13e5" />

<img width="757" height="97" alt="Screenshot 2026-11-10 092150" src="https://github.com/user-attachments/assets/a7aa49bd-2c39-41c1-a32f-a3b70f4a4420" />

### Base Component

It was then time to start building my base component of my fit.

<img width="1456" height="727" alt="Screenshot 2026-11-10 093202" src="https://github.com/user-attachments/assets/34144743-1fe6-4cf4-9e69-e20a98ba2189" />

<img width="1422" height="691" alt="Screenshot 2026-11-10 093240" src="https://github.com/user-attachments/assets/24adf697-e837-46ab-89d2-38a24ab6025d" />

I shelled out the base block to reduce material as well as to create a storage use for the box, making it into a container build.

<img width="1315" height="771" alt="Screenshot 2026-11-10 094201" src="https://github.com/user-attachments/assets/f00184ca-7d01-4cb1-96ce-72a5526d8e7e" />

<img width="1483" height="557" alt="Screenshot 2026-11-10 100138" src="https://github.com/user-attachments/assets/28354249-fe23-4d6d-9908-5c4b45b8b76d" />

The next step was to start to build the receiving latch to the base component. I struggled slightly with getting the latch to rest evenly on the side face. I eventually got it to work.

<img width="901" height="622" alt="Screenshot 2026-11-10 100347" src="https://github.com/user-attachments/assets/4821ac9e-1b3d-4283-b707-0c0db24c217f" />

<img width="1461" height="792" alt="Screenshot 2026-11-10 101325" src="https://github.com/user-attachments/assets/812b5553-78af-4abb-ade3-158accd1a3d2" />

<img width="946" height="751" alt="Screenshot 2026-11-10 103408" src="https://github.com/user-attachments/assets/0dc27384-a973-4bec-ae07-071c8ca90058" />

<img width="607" height="677" alt="Screenshot 2026-11-10 105050" src="https://github.com/user-attachments/assets/1c4a36ea-c445-4309-8fcf-25a16018939c" />

<img width="481" height="873" alt="Screenshot 2026-11-10 105356" src="https://github.com/user-attachments/assets/76b71ac0-96c3-4657-a8e9-b8a863746752" />

<img width="530" height="667" alt="Screenshot 2026-11-10 105536" src="https://github.com/user-attachments/assets/fc095dc7-484c-430c-a472-778e187f3669" />

My latch was very thin on where it joined to the extruded rectangular area. I worried about this sustaining itself when printing, so I asked AI if it believed it would fail when it came time to print my piece. It did not believe there was any worry with my orientation, so I proceeded(it would end up being wrong).

### Lid Component

The next step was to begin to design the lid component of the fit. This lid would feature the whole in which the clamp would snap into.

<img width="777" height="615" alt="Screenshot 2026-11-10 110128" src="https://github.com/user-attachments/assets/a70aec68-9540-464c-9762-b747cbc6a559" />

<img width="963" height="590" alt="Screenshot 2026-11-10 110151" src="https://github.com/user-attachments/assets/c685b27e-74e6-4285-aef7-f3489e613ffa" />

<img width="866" height="797" alt="Screenshot 2026-11-10 110855" src="https://github.com/user-attachments/assets/f5a4d43f-9483-4dc5-8435-b1285ab1bfc6" />

<img width="1067" height="790" alt="Screenshot 2026-11-10 110956" src="https://github.com/user-attachments/assets/42202027-e203-4b79-bba8-62338e5c20d5" />

I had originally intended for the lid to be closed so that container encloses whatever it holds with no light or open air. However, I decided to remove the top face of the lid in a fear that the mating features of the fit will fail and extra resources and time will be used. So for a rough prototype I removed this top face.

<img width="748" height="656" alt="Screenshot 2026-11-10 111331" src="https://github.com/user-attachments/assets/42508745-1770-4b1d-947e-8a044d5b8185" />

<img width="763" height="512" alt="Screenshot 2026-11-10 111811" src="https://github.com/user-attachments/assets/a2f0ea40-095c-4dc1-9e82-1e18315b97a1" />

<img width="817" height="596" alt="Screenshot 2026-11-10 112553" src="https://github.com/user-attachments/assets/36e62922-06cb-42ec-a663-44b3d1f58ae9" />

<img width="1085" height="685" alt="Screenshot 2026-11-10 112737" src="https://github.com/user-attachments/assets/02331c66-854a-4ae7-8c54-1e32adcd0729" />

After my two components were created, I decided to not make an assembly of the feature to see how it would fit. I would later regret this decision.

## Preprocessing

I added the two components into Preform and began to adjust the orientation to get an idea of what the print will look like.

<img width="1501" height="990" alt="Screenshot 2026-11-12 153116" src="https://github.com/user-attachments/assets/96f09618-b399-40ec-9ba7-4b648d13e982" />

Importantly, no structural supports appeared on the mating pieces of either component, which was very important to reduce any rough edges when trying to connect the fit after printing.

<img width="482" height="320" alt="Screenshot 2026-11-12 153128" src="https://github.com/user-attachments/assets/f0b9fb99-f9ff-40ec-a45d-f805260c866e" />

The original printing time was around 2 hours with a normal orientation. To reduce my printing time to near an hour, I scaled down both features to be 0.6 times their original size. I would regret this later on as you will see shortly.

## Printing

<img width="3024" height="4032" alt="IMG_3362" src="https://github.com/user-attachments/assets/52b84611-108f-46f4-a459-5a4d8205e695" />

I printed the build and waited in the FAB Lab for the entirety of the hour and 15 mins of my print time. After it was done, I placed it in the alcohol bath for roughly 5 mins to clean it.

## Post-Processing

I did not manage to take any pictures of the bath or me removing any of the supports. I did manage to accidentally break the rectangular lid as it was very flimsy without that top face on it. 

<img width="3024" height="4032" alt="IMG_3363" src="https://github.com/user-attachments/assets/bae7469c-869f-4a7f-9a05-ed4e053c70c7" />

Another thing that can be observed is how truly small this build was. When I originally scaled down the fits, I thought they would be just large enough for the mating features to show and adjoin to each other. I was very wrong about this as both the clip and the hole feature were so minute that they did no serve much of a purpose at all.

Because of this, I was forced with a decision to redesign my build or start a completely new design. I opted to keep the same nominal idea and make some changes to make the feature available for practical use.

## Rebuilding

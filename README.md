# Sustainability-Paradox-in-Aviation
Sustainability paradox in aviation: the impact of engine design efficiency on contrail formation and environmental sustainability

**1. Introduction**
When we talk about the aviation industry’s role in the climate crisis, the first things that generally come to mind are the amount of carbon emissions from airplanes and the steps needed to offset those emissions. Both news reports and sustainability reports tend to focus primarily on fuel consumption. However, the fact that commercial aviation is contributing to global warming is not limited to these exhaust emissions alone. Another factor—one that most of us actually overlook, even though we often see them in the sky—is those white trails left behind by airplanes, known as contrails (artificial clouds).

Recent research in climate science shows that these artificial clouds could contribute to global warming to a much greater extent than the carbon dioxide emitted by airplanes by trapping heat rising from the Earth at night. It is precisely at this point that a major contradiction (a paradox) arises between engineering and environmental science. Aviation companies have spent billions of dollars developing a new generation of highly efficient engines called High-Bypass to become more environmentally friendly, consume less fuel, and reduce carbon emissions. These engines have successfully reduced carbon emissions. However, as the engines’ efficiency increased, the temperature of the exhaust gases dropped. When cold exhaust gases mix with the freezing atmosphere at high altitudes, they begin to form ice crystals much more easily and create artificial clouds in the sky that lasted much longer. In other words, green engines designed to emit less carbon have actually produced a side effect that has the potential to warm the planet even more.

The primary goal of this project—and what really caught my interest—is precisely to explain this invisible contradiction in a clear and understandable way. To examine this process, I built an interdisciplinary bridge by combining data science (Python), mechanical engineering (engine technologies), and atmospheric physics (cloud microphysics). Unlike the massive 3D simulation models used in the literature that rely on supercomputers, in this study I aimed to demonstrate the 40-year evolutionary trend in the history of civil aviation with a level of transparency and simplicity that anyone can understand by reducing such a complex and chaotic physical system to just two fundamental parameters.

**2. Theoretical Framework and the Schmidt-Appleman Criterion**
In fact, we can use the basic phase changes covered in high school physics and chemistry classes as a foundation for understanding how those white trails behind an airplane form. When a passenger plane’s engine burns fuel, it emits large amounts of water vapor along with carbon dioxide and heat. At the standard cruising altitude of 35,000 feet, the outside air is typically around -50°C.When the hot, moist exhaust gas from the engine comes into contact with this cold atmosphere, it instantly condenses and rapidly turns into tiny ice crystals. In other words, the streaks we see in the sky are actually human-made, artificial clouds.

So how do we predict when these clouds will or won’t form, in other words, what are the limits of this phenomenon? This is where the Schmidt-Appleman Criterion, named after its inventors and widely accepted in atmospheric physics since the 1950s, comes into effect. This criterion models the process by which exhaust gases mix with ambient air in the sky using a thermodynamic line. The slope of this line, which represents the mixing process, determines the threshold for artificial cloud formation and is calculated in atmospheric physics using the following formula:

$$G = \frac{EI_{H_{2}O} \cdot c_p \cdot P_a}{\epsilon \cdot Q \cdot (1 - \eta_o)}$$

Although the letters in the formula may seem confusing, they shouldn’t be intimidating because, with the exception of $$\eta_o$$, all the remaining values represent physical quantities that are fixed according to international standards:

$EI_{H_{2}O}$ (Water Vapour Emissions Index): $1.23 \text{ kg/kg}$ (This is the standard for all civil aircraft using Jet A-1/kerosene fuel).

$c_p$ (Specific Heat of Air): $1004 \text{ J/(kg}\cdot\text{K)}$ (Standard thermodynamic constant).

$\epsilon$ (Molar Mass Ratio): $0.622$ (The ratio of the molar mass of water to that of dry air).

$Q$ (Lower Heating Value of Fuel): $43.2 \times 10^6 \text{ J/kg}$ (The standard chemical energy of aviation kerosene).

$P_a$ (Ambient Pressure): $23842 \text{ Pa}$ (The barometric pressure at an altitude of 35,000 feet [ISA – International Standard Atmosphere], which is the standard cruising altitude for aircraft).

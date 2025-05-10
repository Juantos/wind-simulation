# Wind Generation Simulation with WindPowerLib

The main goal of this project is to simulate wind generation data, compare it with real data and see how close it can get.

## Concepts

### Maximal theoretical power output
$P_{wind} \ \ (Watts)$

$$ P_{wind} = \frac{1}{2} \cdot \rho Av^3 $$

Why is that? The **air mass flow rate** relates to how fast ($v$) some amount of air ($\rho$) is hitting the blades ($A$). **Kinetic energy** moves the air blades, so we multiply them.

$$ Power = \text{mass flow rate} \times \text{energy per mass} $$

$$\text{Air mass flow rate: } \dot{m} = \rho A v$$ 

$$\text{Kinetic energy per unit mass: } \frac{E_k}{m} = \frac{1}{2}v^2 $$

$$ P_{wind} = \frac{1}{2} \cdot \rho Av^3 $$

### Turbine power output
$P_{turbine} \ \ (Watts)$

$$ P_{wind} = \frac{1}{2} \cdot \rho Av^3C_p$$

### Air density
$\rho \ \ (kg/m^3)$

Proportionality between $P_{wind}$ and $\rho$ is linear. Air is denser at sea level than at cloud level, which means the lower the blades, the higher the energy production is (if other variables remain unchanged).

It depends on **pressure**, **tempreature**, and **relative humidity**.

### Turbine blades swept area
$A= \pi r^2 \ \ (m^2) $

Bigger blades capture more energy. It is determined by the **rotor diameter**.

### Wind speed
$v \ \ (m/s^2)$

Main energy input (kinetic), as it affects the power **cubically**.

### Power coefficient
$C_p$ , (dimensionless)

Efficiency of the turbine power conversion. Varies with wind speed and turbine design. Its typical range goes from 0.3 to 0.45, with a theoretical maximum of 0.593 known as **Betz limit**, meaning no wind turbine can capture more than 59.3% of the kinetic energy in the wind. Betz's law is derived from the principles of conservation of mass, momentum and energy.

So, if $C_p = 0.32$, it means the turbine can produce 32% of the theoretical maximum wind energy.

### Hub height

Height of the turbine rotor.

### Yaw angle

Angle between the rotor axis and the wind direction. Usually, turbine use yaw motors to align with wind direction in real time and maximize energy production.

### Wind direction

Compass direction from which the wind blows, determining the turbine orientation.

### Wake losses

The wake is the region of slower and turbulent air behind the turbine, after the air strikes the blades. In consequence, this region has lower-pressure.

The wake zone affects downstream turbines, reducing their power output if they operate within another turbine's wake.

### Turbine power curve

Graph or dataset showing the electrical power output of a turbine as a function of wind speed.
- Cut-in: turbine starts producing power
- Rated speed: delivers max rated power
- Cut-out: shuts down to prevent damage



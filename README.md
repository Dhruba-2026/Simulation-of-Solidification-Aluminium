# Simulation-of-Solidification-Aluminium
Numerical simulation of cooling and solidification behaviour in aluminium alloy using Python (Finite Difference Method).
rho=2700#Density(kg/m^3)
k=180#Thermal Conductivity(W/mk)
cp=900#Specific heat(J/kgK)
l=397000#Latent Heat(J/Kg)
Tm=660#Melting Temp(degree Celcius)
Ti=750#Initial Temp(degree Celcius)
Ta=25#Ambient Temperature(degree celcius)
thickness=0.02#2cm slab(m)
h=20#heat transfer coefficient (W/m^2K) (natural convection assumption)

#Assume 1 m^2 surface area slab
area=1
volume=area*thickness
mass=rho*volume

#
#1. Cooling Rate
#

delta_T=Ti-Ta
cooling_rate= (h*delta_T)/(rho * cp * thickness)

#
#2. Total Heat Removed
#

Q_sensible=mass*cp*(Ti-Tm)
Q_latent=mass*l
Q_total=Q_sensible+Q_latent

#
#3. Thermal Diffusivity
#

alpha=k/(rho*cp)

#Assume approximate solidification time (seconds)
solidification_time=300

#
#4. Fourier Number
#

Fo=(alpha * solidification_time)/(thickness**2)

#
#5. Thermal Gradient
#

thermal_gradient=(Ti-Ta)/thickness

#
#6.Solidification Front Velocity
#

solidification_velocity=cooling_rate/thermal_gradient

#
#Print Results
#

print("===== Numerical Results =====\n")

print(f"Cooling Rate: {cooling_rate:.4f} C/s")

print(f"\nMass of Slab: {mass: .2f} kg")

print(f"\nSensible Heat Removed: {Q_sensible:.2f} J")

print(f"Latent Heat Removed: {Q_latent:.2f} J")

print(f"Total Heat removed: {Q_total:.2f} J")

print(f"\nThermal Diffusivity: {alpha:.6e}m^2/s")

print(f"\nFourier Number: {Fo:.2f}")

print(f"\nThermal Gradient: {thermal_gradient:.2f} K/m")

print(f"\nSolidification Front Velocity: {solidification_velocity:.6e} m/s")

print("\n===== END OF SIMULATION =====")

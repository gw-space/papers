# The problem presented in the paper
The paper presents the issue of 4G/5G mobility management being unstable in situations of high-speed movement, such as on high-speed trains. The fundamental reason for the instability of 4G/5G in extreme mobility is presented as its design based on wireless signal strength. While this method is reasonable in static and low-mobility scenarios, the design is sensitive to the severe wireless dynamics caused by the Doppler shift in extreme mobility. Such dynamics propagate through all stages of mobility management, leading to slow feedback during triggering, missing optimal candidate cells during decision-making, and producing unstable signals during execution.

# Proposed solution
This paper proposes REM, a solution that manages mobility based on the movement of the client rather than wireless signal strength.

# Contribution
1. Conducted an empirical study for the network reliability in extreme mobility. With the datasets from the Chinese high-speed rails.
2. Designed REM, the first movement-based reliable extreme mobility management for 4G, 5G and beyond. As a signaling overlay in the delay-Doppler domain, REM devises SVD-based cross-band estimation to relax the feedback, simplifies the policy for provable conflict freedom, and stabilizes the signaling with scheduling-based OTFS modulation.
3. Prototyped REM using software-de￿ned radio, and systematically evaluate REM’s network failure reduction, policy conflict resolution, and system overhead.

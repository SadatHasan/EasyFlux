# EasyFlux
'LabView based Fluorescence lifetime activated droplet sorting software'

The time trace (top) in the front panel is a continuously generating timeline of photon stream coming from the droplets.
Considering background noise/fluorescence, the threshold for droplet detection can be set by the user.
The Histogram (middle) is generating a histogram of photon decay from the last passing droplet.
The user can set the minimum number of photons from one droplet that will generate a average lifetime.
Setting the threshold too low might widen error margin in the average lifetime calculation.
Setting the threshold too high, photon count might not be sufficient for generating an average lifetime.
Laser intensity has to be optimizied considering dye concentration, droplet size, speed and chip attributes.
t0 is set by user. It is supposed to be set at the point where histogram starts rising followed by the pulsed excitation.
The Lifetime graph (bottom) shows average lifetime value from the last generated histogram.
The average lifetime threshold for actuating droplets is user defined and depending on your dye selection.
In case the droplet has higher lifetime than the threshold, a TTL pulse can be generated by using the tick-mark box beside Lifetime graph.
The front panel shows delay calculation of droplet detection and lifetime calculation.
According to that, a delay can be added on the TTL pulse that actuates the droplet.
TTL pulse width can be varied to sync with your experimental setup.
The block diagram gives the complete program structure and code, user can modifiy it if necessary.
It is shown in the block diagram of the first version, where to implement the DAQ.
In the second version, a basic DAQ is implemented with delay timers for example.

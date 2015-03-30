# wspr
WSPR related code snippets and tools

Several tools based on online sources for implementing wspr on raspberry pi and arduino

******
Credits:
******
  Wspr encoding portion is adapted from james [4] &  Guido PE1NNZ [3]
  Oliver Mattos and Oskar Weigl who implemented PiFM [1]
  Dan MD1CLV combined this effort with WSPR encoding algorithm from F8CHK,
  resulting in WsprryPi a WSPR beacon for LF and MF bands.
  Guido PE1NNZ <pe1nnz@amsat.org> extended this effort with DMA based PWM
  modulation of fractional divider that was part of PiFM, allowing to operate
  the WSPR beacon also on HF and VHF bands.  In addition time-synchronisation
  and double amount of power output was implemented.
  James Peroulas <james@peroulas.com> added several command line options, a
  makefile, improved frequency generation precision so as to be able to
  precisely generate a tone at a fraction of a Hz, and added a self calibration
  feature where the code attempts to derrive frequency calibration information
  from an installed NTP deamon.  Furthermore, the TX length of the WSPR symbols
  is more precise and does not vary based on system load or PWM clock
  frequency.
  Michael Tatarinov for adding a patch to get PPM info directly from the
  kernel.
  
  [1] PiFM code from
      http://www.icrobotics.co.uk/wiki/index.php/Turning_the_Raspberry_Pi_Into_an_FM_Transmitter
  [2] Original WSPR Pi transmitter code by Dan:
      https://github.com/DanAnkers/WsprryPi
  [3] Fork created by Guido:
      https://github.com/threeme3/WsprryPi
  [4] https://github.com/JamesP6000/WsprryPi

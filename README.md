<h3>Project Overview</h3>

<p>
  This experiment investigates the behavior of a <strong>DC machine</strong> using
  different rectifier configurations. The study examines the relationship between
  the <strong>firing angle, rectified voltage, current, and machine speed</strong>.
  Experimental results are compared with theoretical models to evaluate the effects
  of rectification and additional components such as a <strong>freewheeling diode</strong>
  and a <strong>smoothing inductor</strong>.
</p>

<h3>Objectives</h3>
<ul>
  <li>
    Study the <strong>conduction mode</strong> for an RLE active load and the
    smoothing effect on the rectified current.
  </li>
  <li>
    Analyze the effect of a <strong>freewheeling diode (FWD)</strong> on the
    rectified current and conduction mode.
  </li>
  <li>
    Study the <strong>speed control characteristics</strong> and speed variation
    of the DC machine.
  </li>
</ul>
<h3>Theoretical Background</h3>
<p>
  A <strong>single-phase thyristor bridge</strong>, also known as a
  <strong>full-wave thyristor rectifier</strong>, is a power electronic circuit
  used to convert AC voltage into DC voltage. By adjusting the
  <strong>thyristor firing angle</strong>, the portion of the AC waveform being
  rectified can be controlled, thereby regulating the output DC voltage and current.
</p>
<p align="center">
  <img src="image167.jpg"
       alt="Single-Phase Thyristor Bridge"
       width="900">
</p>
<p>
  The <strong>thyristor rectifier</strong> performs a controlled
  <strong>AC-to-DC conversion</strong>. Control is achieved by adjusting the
  <strong>firing delay angle</strong>. The thyristors operate in pairs:
  <strong>(T1 and T1′)</strong> and <strong>(T2 and T2′)</strong>.
  By varying the firing angle, two distinct conduction modes can be obtained:
  <strong>continuous conduction</strong> and <strong>discontinuous conduction</strong>,
  with the other parameters kept fixed.
</p>

<p>
  For a fixed excitation of the machine field winding, the back electromotive
  force can be expressed as:
</p>

<p align="center">
  <strong>E = K&phi;&Omega; = h&Omega;</strong>
</p>

<p>
  The conduction mode depends on the <strong>firing angle</strong>,
  the <strong>back EMF E</strong>, and the parameter:
</p>

<p align="center">
  <strong>Q = L&omega; / R</strong>
</p>
<h3>Operating Mode</h3>

<h4>Continuous Conduction Mode</h4>

<p>
  In continuous conduction mode, each pair of thyristors conducts for a duration
  of <strong>&pi;</strong>.
</p>

<ul>
  <li>
    For <strong>&omega;t &isin; [&alpha;, &alpha; + &pi;]</strong>:
    <strong>Th1</strong> and <strong>Th1′</strong> are conducting.
    <br>
    <strong>u<sub>d</sub> = u</strong> and
    <strong>i<sub>s</sub> = i<sub>d</sub></strong>.
  </li>

  <li>
    For <strong>&omega;t &isin; [&alpha; + &pi;, &alpha; + 2&pi;]</strong>:
    <strong>Th2</strong> and <strong>Th2′</strong> are conducting.
    <br>
    <strong>u<sub>d</sub> = −u</strong> and
    <strong>i<sub>s</sub> = −i<sub>d</sub></strong>.
  </li>
</ul>
<p align="center">
  <img src="image166.jpg"
       alt="continuous conduction mode rectified voltage and current waveforms"
       width="900">
</p>
<h4>Average Value of the Rectified Voltage</h4>

<p>
  In continuous conduction mode, the average value of the rectified output
  voltage is given by:
</p>

<p align="center">
  <strong>
    &lt;U<sub>d</sub>&gt; =
    (1/&pi;) &int;<sub>&alpha;</sub><sup>&alpha;+&pi;</sup>
    U<sub>m</sub> sin(&omega;t) d(&omega;t)
  </strong>
</p>

<p align="center">
  <strong>
    &lt;U<sub>d</sub>&gt; =
    (2U<sub>m</sub>/&pi;) cos(&alpha;)
  </strong>
</p>

<h4>Discontinuous Conduction Mode</h4>

<p>
  In discontinuous conduction mode, the conduction duration of the thyristors
  is shorter than <strong>&pi;</strong>. The thyristors stop conducting before
  the next pair is triggered.
</p>

<ul>
  <li>
    <strong>Th1</strong> and <strong>Th1′</strong> conduct during their
    corresponding conduction interval.
  </li>
</ul>
<p align="center">
  <img src="image151.jpg"
       alt="Discontinuous conduction mode rectified voltage and current waveforms"
       width="900">
</p>
<h4>Average Value of the Rectified Voltage</h4>

<p>
  In discontinuous conduction mode, the average value of the rectified voltage
  can be expressed as:
</p>

<p align="center">
  <strong>
    &lt;U<sub>d</sub>&gt; =
    (1/2&pi;)
    &left[
      &int; U<sub>m</sub> sin(&omega;t) d(&omega;t)
      + &int; E d(&omega;t)
    &right]
  </strong>
</p>

<p align="center">
  <strong>
    &lt;U<sub>d</sub>&gt; =
    U<sub>m</sub>
    &left[
      cos(&alpha;) - cos(&beta;)
      + K(&beta; - &alpha;)
    &right]
  </strong>
</p>
<h3>Experimental Setup</h3>
<table>
  <thead>
    <tr>
      <th>Equipment</th>
      <th>Image</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Smoothing Inductor (DL 2091 – De Lorenzo)</strong></td>
      <td>
        <img src="image162.jpg"
             alt="Smoothing Inductor DL 2091 De Lorenzo"
             width="200">
      </td>
      <td>
        Used to smooth the rectified current and reduce current ripple in the
        DC machine circuit.
      </td>
    </tr>
    <tr>
      <td><strong>Distribution Box (DL 2308 – De Lorenzo)</strong></td>
      <td>
        <img src="image155.jpg"
             alt="Distribution Box DL 2308 De Lorenzo"
             width="200">
      </td>
      <td>
        Used to provide electrical connections between the different components
        of the experimental setup and facilitate circuit configuration.
      </td>
    </tr>
    <tr>
      <td><strong>Oscilloscope</strong></td>
      <td>
        <img src="image164.jpg"
             alt="Oscilloscope"
             width="200">
      </td>
      <td>
        Used to observe and analyze the voltage and current waveforms during
        the experiment, particularly the rectification and commutation effects.
      </td>
    </tr>
  </tbody>
</table>

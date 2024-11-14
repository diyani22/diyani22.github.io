---
layout: page
title: "OCR"
---
<style>
  /* CSS for two-column layout */
.two-columns {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  border-left: none; /* Removes any border outlines */
  border-right: none; /* Removes any border outlines */
  align-items: start;
  padding: 0;
  margin: 0;
}

.column {
  flex: 1;
  padding: 10px;
  /* Add a border between columns (for the right side of the first column) */
}

.column:not(:last-child) {
  border-right: 1px solid #ddd; /* Add a line between the columns */
}

@media (max-width: 768px) {
  .two-columns {
    flex-direction: column;
  }
  .column {
    border-right: none; /* Remove line between columns on small screens */
  }
}

</style>


<div class="two-columns">
  <div class="column">
    <h2>Paper 1</h2>
    <ul>
      <li><a href="{{ site.baseurl }}/papers/2023%20Paper%201%20QP.pdf" target="_blank">2023 Question Paper</a></li>
      <li><a href="">2023 Mark Scheme</a></li>
      <li><a href="">2023 Model Solutions</a></li>
      <p> </p>
      <li><a href="">2022 Question paper</a></li>
      <li><a href="">2022 Mark Scheme</a></li>
      <li><a href="">2022 Model Solutions</a></li>
      <p> </p>
      <li><a href="">Sample Question paper</a></li>
      <li><a href="">Sample Mark Scheme</a></li>
      <li><a href="">Sample Model Solutions</a></li>
    </ul>
  </div>
  <div class="column">
    <h2>Paper 2</h2>
    <ul>
      <li><a href="">2023 Question paper</a></li>
      <li><a href="">2023 Mark Scheme</a></li>
      <li><a href="">2023 Model Solutions</a></li>
      <p> </p>
      <li><a href="">2022 Question paper</a></li>
      <li><a href="">2022 Mark Scheme</a></li>
      <li><a href="">2022 Model Solutions</a></li>
      <p> </p>
      <li><a href="">Sample Question paper</a></li>
      <li><a href="">Sample Mark Scheme</a></li>
      <li><a href="">Sample Model Solutions</a></li>
    </ul>
  </div>
</div>

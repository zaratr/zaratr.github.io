<tbody><tr>
<th style="text-align:center;">Step</th>
<th style="text-align:center;">Traversal</th>
<th style="text-align:center;">Description</th>
</tr>
<tr>
<td class="ts" style="width:5%;">1</td>
<td style="width:50%"><img src="/data_structures_algorithms/images/bfs_one.jpg" alt="Breadth First Search Step One"></td>
<td style="vertical-align:middle;">Initialize the queue.</td>
</tr>
<tr>
<td class="ts" style="width:5%;">2</td>
<td style="width:50%"><img src="/data_structures_algorithms/images/bfs_two.jpg" alt="Breadth First Search Step Two"></td>
<td style="vertical-align:middle;">We start from visiting <b>S</b> (starting node), and mark it as visited.</td>
</tr>
<tr>
<td class="ts" style="width:5%;">3</td>
<td style="width:50%"><img src="/data_structures_algorithms/images/bfs_three.jpg" alt="Breadth First Search Step Three"></td>
<td style="vertical-align:middle;">We then see an unvisited adjacent node from <b>S</b>. In this example, we have three nodes but alphabetically we choose <b>A</b>, mark it as visited and enqueue it.</td>
</tr>
<tr>
<td class="ts" style="width:5%;">4</td>
<td style="width:50%"><img src="/data_structures_algorithms/images/bfs_four.jpg" alt="Breadth First Search Step Four"></td>
<td style="vertical-align:middle;">Next, the unvisited adjacent node from <b>S</b> is <b>B</b>. We mark it as visited and enqueue it.</td>
</tr>
<tr>
<td class="ts" style="width:5%;">5</td>
<td style="width:50%"><img src="/data_structures_algorithms/images/bfs_five.jpg" alt="Breadth First Search Step Five"></td>
<td style="vertical-align:middle;">Next, the unvisited adjacent node from <b>S</b> is <b>C</b>. We mark it as visited and enqueue it.</td>
</tr>
<tr>
<td class="ts" style="width:5%;">6</td>
<td style="width:50%"><img src="/data_structures_algorithms/images/bfs_six.jpg" alt="Breadth First Search Step Six"></td>
<td style="vertical-align:middle;">Now, <b>S</b> is left with no unvisited adjacent nodes. So, we dequeue and find <b>A</b>.</td>
</tr>
<tr>
<td class="ts" style="width:5%;">7</td>
<td style="width:50%"><img src="/data_structures_algorithms/images/bfs_seven.jpg" alt="Breadth First Search Step Seven"></td>
<td style="vertical-align:middle;">From <b>A</b> we have <b>D</b> as unvisited adjacent node. We mark it as visited and enqueue it.</td>
</tr>
</tbody>

<script lang="ts">
	import { onMount } from 'svelte';

	let selectedTable = 'table1';

	onMount(() => {
		const tableSelect = document.getElementById('table-select');

		// Hide all tables initially
		const tables = document.querySelectorAll('table');
		tables.forEach((table) => {
			table.style.display = 'none';
		});

		if (tableSelect) {
			// Show the selected table based on the option
			tableSelect.addEventListener('change', () => {
				const selectedTableId = (tableSelect as HTMLSelectElement).value;

				tables.forEach((table) => {
					if (table.id === selectedTableId) {
						table.style.display = 'table';
					} else {
						table.style.display = 'none';
					}
				});
			});
		}

		// Show the first table by default if available
		const firstTable = document.getElementById('table1');
		if (firstTable) {
			firstTable.style.display = 'table';
		}
	});
</script>

<div class="grid grid-cols-1 lg:grid-cols-3 p-5 max-w-7xl mx-auto">
	<div class="m-auto text-2xl font-bold">2023.Gada rezultāti</div>
	<div class=" col-end-6 flex m-auto lg:mr-0 p-2 lg:m-auto">
		<select id="table-select" class="select select-primary w-full max-w-xs">
			<option value="table1">Nakts Auto Orientēšanās</option>
			<option value="table2">Ātruma Aplis</option>
			<option>Dragreiss</option>
			<option>Decibelu dragreiss</option>
			<option>Skaistuma konkurss</option>
			<option>Drifts</option>
			<option>Veiklības brauciens</option>
		</select>
	</div>
</div>

<!-- NAKTS AUTO ORIENTEŠANAS -->
<div class="overflow-x-auto p-10 pt-5 pb-0 max-w-7xl mx-auto">
	<table id="table1" class="table table-xs">
		<thead>
			<tr>
				<th class="text-lg">Vieta</th>
				<th class="text-lg">Dalībnieka Nr.</th>
			</tr>
		</thead>
		<tbody>
			<tr>
				<td>1. vieta</td>
				<td>002</td>
			</tr>
			<tr>
				<td>2. vieta</td>
				<td>021</td>
			</tr>
			<tr>
				<td>3. vieta</td>
				<td>018</td>
			</tr>
			<tr>
				<td>4. vieta</td>
				<td>000</td>
			</tr>
			<tr>
				<td>5. vieta</td>
				<td>009</td>
			</tr>
			<tr>
				<td>6. vieta</td>
				<td>012</td>
			</tr>
			<tr>
				<td>7. vieta</td>
				<td>036</td>
			</tr>
			<tr>
				<td>8. vieta</td>
				<td>032</td>
			</tr>
			<tr>
				<td>9. vieta</td>
				<td>015</td>
			</tr>
			<tr>
				<td>10. vieta</td>
				<td>033</td>
			</tr>
			<tr>
				<td>11. vieta</td>
				<td>035</td>
			</tr>
			<tr>
				<td>12. vieta</td>
				<td>026</td>
			</tr>
			<tr>
				<td>13. vieta</td>
				<td>030</td>
			</tr>
			<tr>
				<td>14. vieta</td>
				<td>024</td>
			</tr>
			<tr>
				<td>15. vieta</td>
				<td>010</td>
			</tr>
			<tr>
				<td>16. vieta</td>
				<td>025</td>
			</tr>
			<tr>
				<td>17. vieta</td>
				<td>004</td>
			</tr>
			<tr>
				<td>18. vieta</td>
				<td>039</td>
			</tr>
			<tr>
				<td>19. vieta</td>
				<td>011</td>
			</tr>
			<tr>
				<td>20. vieta</td>
				<td>041</td>
			</tr>
			<tr>
				<td>21. vieta</td>
				<td>027</td>
			</tr>
			<tr>
				<td>22. vieta</td>
				<td>007</td>
			</tr>
			<tr>
				<td>23. vieta</td>
				<td>023</td>
			</tr>
			<tr>
				<td>24. vieta</td>
				<td>008</td>
			</tr>
			<tr>
				<td>25. vieta</td>
				<td>001</td>
			</tr>
			<tr>
				<td>26. vieta</td>
				<td>005</td>
			</tr>
			<tr>
				<td>27. vieta</td>
				<td>006</td>
			</tr>
			<tr>
				<td>28. vieta</td>
				<td>028</td>
			</tr>
			<tr>
				<td>29. vieta</td>
				<td>029</td>
			</tr>
			<tr>
				<td>30. vieta</td>
				<td>040</td>
			</tr>
			<tr>
				<td>31. vieta</td>
				<td>019</td>
			</tr>
			<tr>
				<td>32. vieta</td>
				<td>014</td>
			</tr>
			<tr>
				<td>33. vieta</td>
				<td>034</td>
			</tr>
			<tr>
				<td>34. vieta</td>
				<td>022</td>
			</tr>
			<tr>
				<td>35. vieta</td>
				<td>042</td>
			</tr>
			<tr>
				<td>36. vieta</td>
				<td>031</td>
			</tr>
		</tbody>
		<tfoot>
			<tr>
				<th>Vieta</th>
				<th>Dalībnieka Nr.</th>
			</tr>
		</tfoot>
	</table>
</div>
<!--  ATRUMA APLIS -->
<div class="overflow-x-auto p-10 pt-5 pb-0">
	<table id="table2" class="table table-xs">
		<thead>
			<tr>
				<td class="border-r-2" />
				<td class="text-lg">RWD</td>
				<td class="border-r-2" />
				<td class="text-lg">FWD</td>
				<td class="border-r-2" />
				<td class="text-lg">AWD</td>
				<td />
			</tr>
			<tr>
				<th class=" border-r-2 text-lg text-center">Vieta</th>
				<th class="text-lg">Dalībnieka Nr.</th>
				<th class="text-lg border-r-2">Laiks</th>
				<th class="text-lg">Dalībnieka Nr.</th>
				<th class="text-lg border-r-2">Laiks</th>
				<th class="text-lg">Dalībnieka Nr.</th>
				<th class="text-lg">Laiks</th>
			</tr>
		</thead>
		<tbody>
			<tr>
				<td class="border-r-2 text-center">1</td>
				<td>153</td>
				<td class="border-r-2">0:56:38</td>
				<td>119</td>
				<td class="border-r-2">0:57:13</td>
				<td>080</td>
				<td>0:54:44</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">2</td>
				<td>069</td>
				<td class="border-r-2">0:57:85</td>
				<td>106</td>
				<td class="border-r-2">0:57:35</td>
				<td>177</td>
				<td>0:55:68</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">3</td>
				<td>158</td>
				<td class="border-r-2">0:58:25</td>
				<td>105</td>
				<td class="border-r-2">0:57:97</td>
				<td>333</td>
				<td>0:56:22</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">4</td>
				<td>126</td>
				<td class="border-r-2">0:58:35</td>
				<td>134</td>
				<td class="border-r-2">0:58:82</td>
				<td>162</td>
				<td>0:57:31</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">5</td>
				<td>180</td>
				<td class="border-r-2">0:58:50</td>
				<td>120</td>
				<td class="border-r-2">0:59:34</td>
				<td>155</td>
				<td>0:57:47</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">6</td>
				<td>152</td>
				<td class="border-r-2">0:59:27</td>
				<td>151</td>
				<td class="border-r-2">0:59:44</td>
				<td>076</td>
				<td>0:57:82</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">7</td>
				<td>049</td>
				<td class="border-r-2">0:59:31</td>
				<td>138</td>
				<td class="border-r-2">1:00:02</td>
				<td>046</td>
				<td>0:58:78</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">8</td>
				<td>072</td>
				<td class="border-r-2">0:59:97</td>
				<td>067</td>
				<td class="border-r-2">1:00:38</td>
				<td>127</td>
				<td>0:59:08</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">9</td>
				<td>178</td>
				<td class="border-r-2">1:00:69</td>
				<td>050</td>
				<td class="border-r-2">1:00:47</td>
				<td>154</td>
				<td>1:01:28</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">10</td>
				<td>173</td>
				<td class="border-r-2">1:01:10</td>
				<td>116</td>
				<td class="border-r-2">1:00:60</td>
				<td>145</td>
				<td>1:03:25</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">11</td>
				<td>131</td>
				<td class="border-r-2">1:01:19</td>
				<td>118</td>
				<td class="border-r-2">1:01:38</td>
				<td>170</td>
				<td>1:04:38</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">12</td>
				<td>172</td>
				<td class="border-r-2">1:02:15</td>
				<td>071</td>
				<td class="border-r-2">1:02:03</td>
				<td>169</td>
				<td>1:07:47</td>
			</tr>
			<tr>
				<td class="border-r-2 text-center">13</td>
				<td>168</td>
				<td class="border-r-2">1:02:28</td>
				<td>141</td>
				<td>1:02:60</td>
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">14</td>
				<td>112</td>
				<td class="border-r-2">1:02:40</td>
				<td>123</td>
				<td>1:04:56</td>
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">15</td>
				<td>147</td>
				<td class="border-r-2">1:02:47</td>
				<td>164</td>
				<td>1:05:69</td>
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">16</td>
				<td>128</td>
				<td class="border-r-2">1:03:13</td>
				<td>132</td>
				<td>1:06:85</td>
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">17</td>
				<td>175</td>
				<td class="border-r-2">1:03:22</td>
				<td>171</td>
				<td>1:07:79</td>
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">18</td>
				<td>111</td>
				<td class="border-r-2">1:03:43</td>
				<td>121</td>
				<td>1:09:69</td>
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">19</td>
				<td>177</td>
				<td class="border-r-2">1:03:47</td>
				<td>141</td>
				<td>1:19:13</td>
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">20</td>
				<td>109</td>
				<td>1:03:53</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">21</td>
				<td>053</td>
				<td>1:03:85</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">22</td>
				<td>048</td>
				<td>1:04:16</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">23</td>
				<td>150</td>
				<td>1:04:28</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">24</td>
				<td>140</td>
				<td>1:04:50</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">25</td>
				<td>144</td>
				<td>1:04:53</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">26</td>
				<td>165</td>
				<td>1:04:53</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">27</td>
				<td>136</td>
				<td>1:05:06</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">28</td>
				<td>124</td>
				<td>1:05:71</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">29</td>
				<td>166</td>
				<td>1:05:91</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">30</td>
				<td>110</td>
				<td>1:07:69</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">31</td>
				<td>179</td>
				<td>1:08:25</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">32</td>
				<td>146</td>
				<td>1:08:75</td>
				<td />
				<td />
				<td />
				<td />
			</tr>
			<tr>
				<td class="border-r-2 text-center">33</td>
				<td>159</td>
				<td>1:09:34</td>
				<td />
				<td />
				<td />
				<td />
			</tr>

			<tr>
				<td class="border-r-2 text-center">34</td>

				<td>182</td>
				<td>1:11:75</td>
				<td />
				<td />
			</tr>
		</tbody>
		<tfoot>
			<tr>
				<th>Vieta</th>
				<th>Dalībnieka Nr.</th>
				<th>Laiks</th>
				<th>Dalībnieka Nr.</th>
				<th>Laiks</th>
				<th>Dalībnieka Nr.</th>
				<th>Laiks</th>
			</tr>
		</tfoot>
	</table>
</div>

<style>
	.div {
		max-width: 8xl;
	}
</style>

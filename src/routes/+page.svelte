<script>
	const getCurrentTimeDate = () => {
		let currentTimeDate = new Date();

		var weekday = new Array(7);
		weekday[0] = 'SUN';
		weekday[1] = 'MON';
		weekday[2] = 'TUE';
		weekday[3] = 'WED';
		weekday[4] = 'THU';
		weekday[5] = 'FRI';
		weekday[6] = 'SAT';

		var month = new Array();
		month[0] = 'JAN';
		month[1] = 'FEB';
		month[2] = 'MAR';
		month[3] = 'APR';
		month[4] = 'May';
		month[5] = 'JUN';
		month[6] = 'JUL';
		month[7] = 'AUG';
		month[8] = 'SEP';
		month[9] = 'OCT';
		month[10] = 'NOV';
		month[11] = 'DEC';

		var hours = currentTimeDate.getHours();

		var minutes = currentTimeDate.getMinutes();
		// minutes = minutes < 10 ? '0' + minutes : minutes;

		if (minutes < 10) {
			minutes = '0' + minutes;
		} else {
			minutes = minutes;
		}

		var AMPM = hours >= 12 ? 'PM' : 'AM';

		if (hours === 12) {
			hours = 12;
		} else {
			hours = hours % 12;
		}

		var currentTime = `${hours}:${minutes}${AMPM}`;
		var currentDay = weekday[currentTimeDate.getDay()];

		var currentDate = currentTimeDate.getDate();
		var currentMonth = month[currentTimeDate.getMonth()];
		var CurrentYear = currentTimeDate.getFullYear();

		var fullDate = `${currentDate} ${currentMonth} ${CurrentYear}`;

		document.getElementById('time').innerHTML = currentTime;
		document.getElementById('day').innerHTML = currentDay;
		document.getElementById('date').innerHTML = fullDate;

		setTimeout(getCurrentTimeDate, 500);
	};

	getCurrentTimeDate();
</script>

<body>
	<h1>Hi, I'm Syed</h1>
	<h2>Developer | Student | Founder</h2>
	<div class="content">
		I'm a 15 year old builder who makes cool stuff if I can focus. I've worked for and founded a
		couple of agencies and startups. I'm a freelance developer, designer, marketer and writer. <br
		/>
		I'm currently busy creating an AI consulting company called <i> firstgenesis </i> . <br />
		I'm interested in the intersection of the arts and humanities with technology and science, particularly
		buidling user-friendly but extremely effecient products and systems. I'm a philomath, philosopher
		and liberal (the classical meaning, not the modern one). I'm religous but skeptical. Welcome to my
		corner of the internet.
	</div>

	<div>
		<p id="time">1:20PM</p>
		<p id="day">SUN</p>
		<p id="date">9 May 2021</p>
	</div>
</body>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Montserrat&family=Raleway:wght@600&display=swap');
	body {
		background: #14191a;
		color: white;
		font-family: 'Montserrat', sans-serif;
		font-family: 'Raleway', sans-serif;
		display: flex;
		flex-direction: column;
		justify-content: center;
	}
	h2 {
		font-size: 1em;
		color: grey;
		line-height: 1px;
		margin-top: 1px;
		margin-bottom: 2em;
	}

	.content {
		line-height: 2em;
	}

	p {
		display: inline;
		margin: 5px;
	}

	#time {
		font-size: 60px;
		color: #004aad;
	}

	#day {
		font-size: 40px;
		color: #ff5757;
	}

	#date {
		font-size: 20px;
		color: #ff5757;
	}
</style>

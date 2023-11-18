# Astro Data Sources

- Get internal or exertnal data sources
- Diplay data sources
- 3 different options to get data sources
    - Option 1: Internal Frontmatter
    - Option 2: Local data files
    - Option 3: External data


const dataSource = 'https://gist.githubusercontent.com/ewuweblab/b8c52837370e6e39b3603dea2d0f6a07/raw/ee24073bada30f1a99b1bdfde81e05d389eb120e/emojiHolidays.json';
const response = await fetch(dataSource);
const emojiHolidays = await response.json();



			{ 
				emojiHolidays.map( holiday => (
			
					<li>
						{ holiday.emoji } { holiday.name }  
					</li>
					
					)
				)
			}	
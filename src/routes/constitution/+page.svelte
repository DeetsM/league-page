<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneOneOne, oneTwo, oneTwoOne, oneTwoTwo, oneTwoThree, oneThree;
    let two, twoOne, twoTwo;
    let three, threeOne, threeTwo;
    let four, fourOne, fourTwo;
    let five, fiveOne, fiveTwo;
    let six, sixOne, sixTwo;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p {
        color: #777;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">LEGENDS LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(one)}>Section 1: Roster</h3>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneOne)}>1.1 Positional Breakdown</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneTwo)}>1.2 Trading</h4>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoOne)}>1.2.1 Trade Deadline</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoFour)}>1.2.2 Trade Restrictions</h5>
            <h5 class="noUnderscore clickable" onclick={() => goToSection(oneTwoFive)}>1.2.3 Vetoing Trades</h5>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(oneThree)}>1.3 Waiver Wire</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(two)}>Section 2: Drafting</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoOne)}>2.1 Draft Date/Location</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(twoTwo)}>2.2 Draft Order</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(three)}>Section 3: Keepers</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(threeOne)}>3.1 Keepers</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(threeTwo)}>3.2 Locking in Keepers</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(four)}>Section 4: Scoring System</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourOne)}>4.1 Scoring System</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fourTwo)}>4.2 Random Scoring</h4>
    
    <h3 class="noUnderscore clickable" onclick={() => goToSection(five)}>Section 5: Postseason</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fiveOne)}>5.1 Playoffs</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(fiveTwo)}>5.2 Playoff Tiebreakers</h4>

    <h3 class="noUnderscore clickable" onclick={() => goToSection(six)}>Section 6: League Finances</h3>
    
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixOne)}>6.1 League Dues</h4>
        <h4 class="noUnderscore clickable" onclick={() => goToSection(sixTwo)}>6.2 Payout</h4>    
    
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Section 1 Roster Breakdown</h2>
    
    <h3 class="subSectionHeading" bind:this={oneOne}>1.1 Positional Breakdown</h3>
    
    <p>15 Total Players</p>
    
    <p class="underscore">Starters</p>
    <ul>
        <li>QB</li>
        <li>RB</li>
        <li>RB</li>
        <li>WR</li>
        <li>WR</li>
        <li>TE</li>
        <li>FLEX (RB/WR/TE)</li>
        <li>D/ST</li>
        <li>K</li>
    </ul>
    
    <p>5 Bench</p>

    <p>2 IR Spots</p>

    <h3 class="subSectionHeading" bind:this={oneTwo}>1.2 Trading</h3>
    
    <p>Trades are allowed up until the trade deadline and also during the offseason. Tradable assets include players, draft picks, and FAAB $.</p>
    
    <h4 bind:this={oneTwoOne}>1.2.1 Trade Deadline</h4>
    <div class="subBlock">
        <p>The trade deadline will be set for week 11 of the NFL season.</p>
    </div>
    
    <h4 bind:this={oneTwoTwo}>1.2.2 Trade Restrictions</h4>
    <div class="subBlock">
        <p>You will not be able to trade draft picks that are in the last 2 rounds of the draft (Rounds 13 and 14) as these are reserved for Keepers.</p>
    </div>
    
    <h4 bind:this={oneTwoThree}>1.2.3 Vetoing Trades</h4>
    <div class="subBlock">
        <p>Vetoes are only appropriate in instances of collusion or an egregious mismatch of value (i.e. CMC for a backup kicker). Not liking a trade does not warrant a veto.</p>
    </div>
    
    <h3 bind:this={oneThree}>1.3 Waiver Wire</h3>
    
    <p>FAAB Waiver wire system. Each team will begin the season with $100 plus carryover. Each team will be able to carry over a maximum of $25 FAAB to the following season. $0 bids are allowed.</p>
    
    <h2 class="sectionHeading" bind:this={two}>Section 2 Drafting</h2>
    
    <h3 bind:this={twoOne}>2.1 Draft Date/Location</h3>
    <p>The draft date and time will be posted on the league website. The time and location of the draft will be determined by league consensus at the league AGM (following the end of the season)</p>

    <h3 bind:this={twoTwo}>2.2 Draft Order</h3>
    <p>The winner of the consolation bracket will get 1st choice of draft position. It will continue based on reverse standings. After the first 4 spots are taken, the remaining choices will go in reverse playoff bracket finish order.</p>
    <p>So the draft order will be (finish placement): 7 > 10 > 9 > 8 > 6 > 5 > 4 > 3 > 2 > 1</p>    
    <p>Any spots not filled during the draft, can be filled immediately afterwards from the free agent pool</p>

    <h2 class="sectionHeading" bind:this={three}>Section 3 Keeper</h2>

    <h3 bind:this={threeOne}>3.1 Keepers</h3>
    <p>Each team is required to keep 2 players from their roster going into the next season</p>
    <p>Keepers are placed at the end of the draft (Rounds 13 and 14).</p>

    <h3 bind:this={threeTwo}>3.2 Locking in Keepers</h3>
    <p>Keepers are locked in mid-May (date to be specified at AGM)</p>

    <h2 class="sectionHeading" bind:this={four}>Section 4 Scoring System</h2>

    <h3 bind:this={fourOne}>4.1 Scoring System</h3>
    <p>The league scoring system breakdown is listed on the Sleeper fantasy app (for the most part, it follows typical PPR Scoring).</p>
    <p>Custom scoring rules are primarily around kickers and defense in order to help balance their value</p>

    <h3 bind:this={fourTwo}>4.2 Random Scoring</h3>
    <p>The league includes a few random circumstance scoring conditions:</p>
    <ol>
        <li>20 points are awarded to a team if their player/defense injures Deshaun Watson</li>
        <li>100 point bonus for a record setting field goal (longest field goal)</li>
    </ol>
    <p>These scores will be manually added to the teams</p>
    
    <h2 class="sectionHeading" bind:this={five}>Section 5 Postseason</h2>
    
    <h3 bind:this={fiveOne}>5.1 Playoffs</h3>
    <p>At the end of the season 6 teams will make the playoffs. The first round of playoffs will commence in week 15. The top two teams in each division and the 2 wild card teams that finish with the best records, will receive a playoff berth. The 2 teams that win their division will receive a bye week in the first round of the playoffs. Each playoff matchup will only last one week and the winner will advance.</p>
    
    <h3 bind:this={fiveTwo}>5.2 Seeding Tiebreakers</h3>
    <p>If two teams finish with the same record the tiebreakers will go as followed:</p>

    <ol>
        <li>Points For</li>
        <li>Head 2 Head Record</li>
        <li>Division Record</li>
        <li>Total Points Against</li>
        <li>Coin Flip</li>
    </ol>

    <p>Teams remain on their side of the bracket through the playoffs</p>

    <h2 class="sectionHeading" bind:this={six}>Section 6 League Finances</h2>
    
    <h3 bind:this={sixOne}>6.1 League Dues</h3>
    <p>League dues are set at {dues}$. Dues are collected through e-transfer to Aditya and will be collected at the draft. All managers must be fully paid up before the start of regular season. In the event that a manager fails to pay before the deadline, their roster is locked until they do so</p>
    
    <h3 bind:this={sixTwo}>6.2 Payout</h3>
    <p>League payout is structured as follows:</p>
    <ul>
        <li>1st place: {dues * 7}$</li>
        <li>2nd place: {dues}$</li>
        <li>3 props: {dues/3}$ each and will be awarded at the end of Weeks 4, 8 and 12 encompassing 4 weeks each (1 - 4, 5 - 8, 9 - 12).</li>
        <li>1 props: {dues/3}$ will be awarded at the end of the regular season that encompasses the entire season.</li>
    </ul>
    <p>Props to be decided befoer the start of the season</p>

</div>

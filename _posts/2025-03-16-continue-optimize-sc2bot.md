---
title: "continue optimize sc2bot"
date: 2025-03-16
---

now can beat all races veryhard level

sometimes can beat zerg CheatInsane level

committing history：<a href="https://github.com/ferryzhou/sc2_bots/commits/main/han">https://github.com/ferryzhou/sc2_bots/commits/main/han</a>

several critical optimizations:
1. enabled micro
2. enable mule in mining
3. enable faster expansion
4. fix placement issues
5. fix some bugs
6. tuned production
7. handle early game cheese

mostly changes are based on prompts + ai code. sometimes need to understand the code and fix some bugs introduced by ai. or do some refactoring.

uploaded bot to ai arena. let's see what happens.

there's still some room to improve.

<h3>Commits on Mar 15, 2025</h3>

<ul>
<li><h4><a title="add run.py for hanbot." href="https://github.com/ferryzhou/sc2_bots/commit/30abb3108e47f5b97a6c1e5d5c9248a0f006e19f">add run.py for hanbot.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed23 minutes ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/30abb3108e47f5b97a6c1e5d5c9248a0f006e19f">30abb31</a></li>
<li><h4><a title="remove some prints." href="https://github.com/ferryzhou/sc2_bots/commit/2ee2fbcb2ff6033834da7c7fd8594203a0383c2b">remove some prints.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed38 minutes ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/2ee2fbcb2ff6033834da7c7fd8594203a0383c2b">2ee2fbc</a></li>
<li><h4><a title="enable handling opponent cheese. some prompts: &quot;in early defense mode, attack opponent structures that have attacking capability (like cannon) and opponent workers first.&quot; &quot;in early defense mode, attack opponent structures that have attacking capability (like cannon) and opponent workers first.&quot;, &quot;in early defense mode, attack opponent structures that have attacking capability (like cannon) and opponent workers first.&quot;" href="https://github.com/ferryzhou/sc2_bots/commit/3b3df9e4739e4645c75d4ec11ba4230ec683f880">enable handling opponent cheese. some prompts: &quot;in early defense mode, attack opponent structures that have attacking capability (like cannon) and opponent workers first.&quot; &quot;in early defense mode, a…</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed5 hours ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/3b3df9e4739e4645c75d4ec11ba4230ec683f880">3b3df9e</a></li>
<li><h4><a title="tune expand_base. total_minerals &lt; 1000 to total_minerals &lt; 2000 for base skips." href="https://github.com/ferryzhou/sc2_bots/commit/049acd95d27c65e0452d15d61ddf3998d5db7536">tune expand_base. total_minerals &lt; 1000 to total_minerals &lt; 2000 for base skips.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed10 hours ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/049acd95d27c65e0452d15d61ddf3998d5db7536">049acd9</a></li>
<li><h4><a title="update expand_base function. Now can beat veryhard terran. Prompt 1: &quot;optimize base expansion to maximize minerals collection.&quot;. Prompt 2:&quot;for existing_base_locations, also count base in pending.&quot;" href="https://github.com/ferryzhou/sc2_bots/commit/d7dd5f182edee838585f8fd5a94cd9e6bc0c017f">update expand_base function. Now can beat veryhard terran. Prompt 1: &quot;optimize base expansion to maximize minerals collection.&quot;. Prompt 2:&quot;for existing_base_locations, also count base in pending.&quot;</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed11 hours ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/d7dd5f182edee838585f8fd5a94cd9e6bc0c017f">d7dd5f1</a></li>
</ul>

<h3>Commits on Mar 13, 2025</h3>

<ul>
<li><h4><a title="allow two base expansion at the same time. fix tank attacking bug and refactor the function." href="https://github.com/ferryzhou/sc2_bots/commit/ef9d2b38322f94f87800c7939a79810efeee7fd3">allow two base expansion at the same time. fix tank attacking bug and refactor the function.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed2 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/ef9d2b38322f94f87800c7939a79810efeee7fd3">ef9d2b3</a></li>
<li><h4><a title="tune expand_base a little bit to allow faster expansion." href="https://github.com/ferryzhou/sc2_bots/commit/276df0fc0ddd4d05db69c4abde27c8b24698c8d3">tune expand_base a little bit to allow faster expansion.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed2 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/276df0fc0ddd4d05db69c4abde27c8b24698c8d3">276df0f</a></li>
</ul>

<h3>Commits on Mar 12, 2025</h3>

<ul>
<li><h4><a title="Now we can win zerg and protoss veryhard." href="https://github.com/ferryzhou/sc2_bots/commit/8ebf1ba418ef37ee21657b80068443d5f31bd151">Now we can win zerg and protoss veryhard.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed3 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/8ebf1ba418ef37ee21657b80068443d5f31bd151">8ebf1ba</a></li>
<li><h4><a title="fix a iteration counting bug." href="https://github.com/ferryzhou/sc2_bots/commit/1b462a810355dff48d5f866f32988f831adf5a48">fix a iteration counting bug.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed3 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/1b462a810355dff48d5f866f32988f831adf5a48">1b462a8</a></li>
<li><h4><a title="move manage_army out of per 10 iteration step. also leave 20% idle production to prepare for base expansion." href="https://github.com/ferryzhou/sc2_bots/commit/7fc15689e36418b842d5f0408ea356a08879b020">move manage_army out of per 10 iteration step. also leave 20% idle production to prepare for base expansion.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed3 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/7fc15689e36418b842d5f0408ea356a08879b020">7fc1568</a></li>
<li><h4><a title="Add run_local_games.py to have han bot vs lishimin bot." href="https://github.com/ferryzhou/sc2_bots/commit/0fc12d89124a2859a67cb0b30ac66baddc4dad24">Add run_local_games.py to have han bot vs lishimin bot.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed3 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/0fc12d89124a2859a67cb0b30ac66baddc4dad24">0fc12d8</a></li>
<li><h4><a title="build more gas as we have mule mining now." href="https://github.com/ferryzhou/sc2_bots/commit/5289503742721993a1f237b886083e0931c38977">build more gas as we have mule mining now.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed3 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/5289503742721993a1f237b886083e0931c38977">5289503</a></li>
</ul>

<h3>Commits on Mar 11, 2025</h3>

<ul>
<li><h4><a title="lift barracks limit as we have more resources left." href="https://github.com/ferryzhou/sc2_bots/commit/363f1f3bca78ba7bf74b97a7cfed7e9e7d7baf16">lift barracks limit as we have more resources left.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed4 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/363f1f3bca78ba7bf74b97a7cfed7e9e7d7baf16">363f1f3</a></li>
<li><h4><a title="tune nearby enemy range so base can be protected. also tuned barrack techlab vs reactor ratio." href="https://github.com/ferryzhou/sc2_bots/commit/7200eac693d8e25b9d093c72c152a260bbaba864">tune nearby enemy range so base can be protected. also tuned barrack techlab vs reactor ratio.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed4 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/7200eac693d8e25b9d093c72c152a260bbaba864">7200eac</a></li>
</ul>

<h3>Commits on Mar 10, 2025</h3>

<ul>
<li><h4><a title="prompt: when we check &quot;if current bases are saturated&quot;, we should exclude bases that's nearly depleted." href="https://github.com/ferryzhou/sc2_bots/commit/9ab28f35a065d0e6df3a05c2bd2502fbdf0d5a1c">prompt: when we check &quot;if current bases are saturated&quot;, we should exclude bases that's nearly depleted.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed5 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/9ab28f35a065d0e6df3a05c2bd2502fbdf0d5a1c">9ab28f3</a></li>
<li><h4><a title="fix a defense bug. current execute_defense is simply rally." href="https://github.com/ferryzhou/sc2_bots/commit/c779509fae8b386cfb3f21600c475ee32f11981a">fix a defense bug. current execute_defense is simply rally.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed5 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/c779509fae8b386cfb3f21600c475ee32f11981a">c779509</a></li>
<li><h4><a title="simplify fallback attack logic." href="https://github.com/ferryzhou/sc2_bots/commit/0eba30521e2a8370746dae88477dadc2358fac40">simplify fallback attack logic.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed5 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/0eba30521e2a8370746dae88477dadc2358fac40">0eba305</a></li>
<li><h4><a title="simplify execute_defense. also add behavior to avoid idle units in attacking mode." href="https://github.com/ferryzhou/sc2_bots/commit/e1cd227a91af3fe499fc31317fbb030b31765fa7">simplify execute_defense. also add behavior to avoid idle units in attacking mode.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed5 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/e1cd227a91af3fe499fc31317fbb030b31765fa7">e1cd227</a></li>
<li><h4><a title="prompt 1: enable mining with mule.. prompt 2: if found enemies near our base, attack them instead of attack enemy base." href="https://github.com/ferryzhou/sc2_bots/commit/a44c81b5847f2d6106503430fb561455fe6d73b8">prompt 1: enable mining with mule.. prompt 2: if found enemies near our base, attack them instead of attack enemy base.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed5 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/a44c81b5847f2d6106503430fb561455fe6d73b8">a44c81b</a></li>
<li><h4><a title="prompt: enable micro for units." href="https://github.com/ferryzhou/sc2_bots/commit/d7faa3840f145f343ffe01474849e69b208a5a99">prompt: enable micro for units.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed5 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/d7faa3840f145f343ffe01474849e69b208a5a99">d7faa38</a></li>
<li><h4><a title="tune some attack params." href="https://github.com/ferryzhou/sc2_bots/commit/7d8c4806b24578ba6297cbfaa12bd0bd85413cdb">tune some attack params.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed5 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/7d8c4806b24578ba6297cbfaa12bd0bd85413cdb">7d8c480</a></li>
<li><h4><a title="attack if we have significant army value advantage." href="https://github.com/ferryzhou/sc2_bots/commit/a3f10a00cdc95ea7f0967ab4baae7b8b6776fac1">attack if we have significant army value advantage.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committed5 days ago

<a href="https://github.com/ferryzhou/sc2_bots/commit/a3f10a00cdc95ea7f0967ab4baae7b8b6776fac1">a3f10a0</a></li>
</ul>

<h3>Commits on Mar 9, 2025</h3>

<ul>
<li><h4><a title="update should_attack function to check whether we have combat advantage." href="https://github.com/ferryzhou/sc2_bots/commit/270dc13dd50e14c917582773f4a408f111305fd9">update should_attack function to check whether we have combat advantage.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committedlast week

<a href="https://github.com/ferryzhou/sc2_bots/commit/270dc13dd50e14c917582773f4a408f111305fd9">270dc13</a></li>
<li><h4><a title="fix allocation_ratio error introduced by ai. move barracks build after factory." href="https://github.com/ferryzhou/sc2_bots/commit/77bddac514d4488100461eaf6bb56cdafb29137c">fix allocation_ratio error introduced by ai. move barracks build after factory.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committedlast week

<a href="https://github.com/ferryzhou/sc2_bots/commit/77bddac514d4488100461eaf6bb56cdafb29137c">77bddac</a></li>
<li><h4><a title="further update placement function to separate buildings so tank can pass through. prompt: in placement function, leave some room between different structures to allow tank to move out. also change total_barracks &gt;= self.workers.amount // 6 instead of 7." href="https://github.com/ferryzhou/sc2_bots/commit/5cc75ffcf165f46b8d042d3d51c284b69d7aefe8">further update placement function to separate buildings so tank can pass through. prompt: in placement function, leave some room between different structures to allow tank to move out.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committedlast week

<a href="https://github.com/ferryzhou/sc2_bots/commit/5cc75ffcf165f46b8d042d3d51c284b69d7aefe8">5cc75ff</a></li>
<li><h4><a title="tuned shoud_attack parameters." href="https://github.com/ferryzhou/sc2_bots/commit/a3de42a55383fab3b5829497aec506762bb4e56c">tuned shoud_attack parameters.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committedlast week

<a href="https://github.com/ferryzhou/sc2_bots/commit/a3de42a55383fab3b5829497aec506762bb4e56c">a3de42a</a></li>
<li><h4><a title="build medivacs before ravens." href="https://github.com/ferryzhou/sc2_bots/commit/c17c82ae2cec83d5324cf0a19a45f9a9d7939f8e">build medivacs before ravens.</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committedlast week

<a href="https://github.com/ferryzhou/sc2_bots/commit/c17c82ae2cec83d5324cf0a19a45f9a9d7939f8e">c17c82a</a></li>
<li><h4><a title="better placement. previously buildings are too close to each other or too crowded. add_on not considered. prompts: 1. have a funciton to calculate where to place the building, make sure there's enough space between all buildings. and use this function for all buildings placement, including but not limited to barracks, factories, starports etc. also consider add_on space in the beginning. 2. the find_placement seems not working, no building is being built for some reason. 3. get error as above" href="https://github.com/ferryzhou/sc2_bots/commit/ec58f156054b998ee8bea51884dcc9b6875277bb">better placement. previously buildings are too close to each other or too crowded. add_on not considered. prompts: 1. have a funciton to calculate where to place the building, make sure there's eno…</a></h4>

<a href="https://github.com/ferryzhou"><img alt="ferryzhou" width="16" height="16" src="https://avatars.githubusercontent.com/u/290287?v=4&amp;size=32" /></a><a href="https://github.com/ferryzhou/sc2_bots/commits?author=ferryzhou">ferryzhou</a>
committedlast week

<a href="https://github.com/ferryzhou/sc2_bots/commit/ec58f156054b998ee8bea51884dcc9b6875277bb">ec58f15</a></li>
<li><h4><a title="Fixed a attacking army allcoation bug introduced by ai." href="https://github.com/ferryzhou/sc2_bots/commit/c923d2485b9ce1fadbdef8e60599a4d64e187fe2">Fixed a attacking army allcoation bug introduced by ai.</a></h4></li>
</ul>

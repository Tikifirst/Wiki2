---
description: The plugin's configuration files
---

# Plugin's files

## Config

{% code title="config.yml" %}
```yaml
# ChatReaction version 1.8.0 configuration file
debug: false
check_updates: true
reaction_stats:
  track_stats: false
  top_players_size: 100
  hostname: localhost
  port: 3306
  database: chatreaction
  prefix: ''
  username: root
  password: ''
  ssl: false
reaction:
  interval: 500
  time_limit: 30
  players_needed_to_start: 4
  word_character_length: 10
  ignore_case: false
  use_custom_words: true
  split_words_by_line: true
  scramble_custom_words: true
  scramble_at_random: true
  scramble_spaces: false
  disabled_worlds:
  - world_nether
  - world_the_end
  reward_amount: 2
  rewards:
  - eco give @p 500
  - give @p diamondblock 100
messages:
  reaction_start:
  - '&8[&e&lReaction&8] &bHover for the word to type!'
  reaction_start_tooltip: '&f%word%'
  scramble_start:
  - '&8[&e&lReaction&8] &bHover for the word to unscramble!'
  scramble_start_tooltip: '&f%word%'
  reaction_end:
  - '&8[&e&lReaction&8] &cNobody got the word in time &4:('
  scramble_end:
  - '&8[&e&lReaction&8] &cNobody got the word in time &4:('
  - '&cThe word was &f%word%'
  reaction_win:
  - '&8[&e&lReaction&8] &f%player% &awon in &f%time% &aseconds!'
  scramble_win:
  - '&8[&e&lReaction&8] &f%player% &aunscrambled the word &f%word% &ain &f%time% &aseconds!'
hooks:
  qaplugin:
    enabled: true
    hint:
      charge: true
      charge_amount: 100.0
```
{% endcode %}

## Words

Words file is empty by default, This will be the file that you will set your custom words list.

{% code title="worlds.txt" %}
```text

```
{% endcode %}


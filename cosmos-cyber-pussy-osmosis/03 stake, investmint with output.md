```
❯ ls -a
╭────┬─────────────────────┬──────┬──────────┬────────────────╮
│  # │        name         │ type │   size   │    modified    │
├────┼─────────────────────┼──────┼──────────┼────────────────┤
│  0 │ .CFUserTextEncoding │ file │      7 B │ 3 weeks ago    │
│  1 │ .DS_Store           │ file │ 10.0 KiB │ a week ago     │
│  2 │ .Trash              │ dir  │    224 B │ 2 weeks ago    │
│  3 │ .alacritty.yml      │ file │ 30.7 KiB │ 2 weeks ago    │
│  4 │ .cache              │ dir  │     96 B │ 2 weeks ago    │
│  5 │ .config             │ dir  │     64 B │ a week ago     │
│  6 │ .cyber              │ dir  │    128 B │ 2 weeks ago    │
│  7 │ .gitconfig          │ file │    140 B │ a week ago     │
│  8 │ .lesshst            │ file │     20 B │ a week ago     │

❯ pussy query bank balances pussy12jlz63jwry4j3jshxlxwx6aulu6kssf83nsxm9
{"balances":[{"denom":"liquidpussy","amount":"980000000000"},{"denom":"milliampere","amount":"1960000"},{"denom":"millivolt","amount":"784000"},{"denom":"pussy","amount":"20000000000"}],"pagination":{"next_key":null,"total":"0"}}

❯ pussy keys list
[{"name":"video-key","type":"local","address":"pussy12jlz63jwry4j3jshxlxwx6aulu6kssf83nsxm9","pubkey":"{\"@type\":\"/cosmos.crypto.secp256k1.PubKey\",\"key\":\"AlEs5WAVVDNyuBtPC00AI7cwtvTdC4aAkBM6DiYh9bpF\"}"},{"name":"video-key2","type":"local","address":"pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f","pubkey":"{\"@type\":\"/cosmos.crypto.secp256k1.PubKey\",\"key\":\"ArQDFUSK7jQpUPPNV35uxGGGz9j3cGNzOWvAVhG00o9g\"}"}]

❯ pussy keys list | from json
╭───┬────────────┬───────┬──────────────────────────────────────────────┬───────────────────────────────────────────────╮
│ # │    name    │ type  │                   address                    │                    pubkey                     │
├───┼────────────┼───────┼──────────────────────────────────────────────┼───────────────────────────────────────────────┤
│ 0 │ video-key  │ local │ pussy12jlz63jwry4j3jshxlxwx6aulu6kssf83nsxm9 │ {"@type":"/cosmos.crypto.secp256k1.PubKey","k │
│   │            │       │                                              │ ey":"AlEs5WAVVDNyuBtPC00AI7cwtvTdC4aAkBM6DiYh │
│   │            │       │                                              │ 9bpF"}                                        │
│ 1 │ video-key2 │ local │ pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f │ {"@type":"/cosmos.crypto.secp256k1.PubKey","k │
│   │            │       │                                              │ ey":"ArQDFUSK7jQpUPPNV35uxGGGz9j3cGNzOWvAVhG0 │
│   │            │       │                                              │ 0o9g"}                                        │
╰───┴────────────┴───────┴──────────────────────────────────────────────┴───────────────────────────────────────────────╯

❯ pussy keys list | from json
╭───┬────────────┬───────┬──────────────────────────────────────────────┬───────────────────────────────────────────────╮
│ # │    name    │ type  │                   address                    │                    pubkey                     │
├───┼────────────┼───────┼──────────────────────────────────────────────┼───────────────────────────────────────────────┤
│ 0 │ video-key  │ local │ pussy12jlz63jwry4j3jshxlxwx6aulu6kssf83nsxm9 │ {"@type":"/cosmos.crypto.secp256k1.PubKey","k │
│   │            │       │                                              │ ey":"AlEs5WAVVDNyuBtPC00AI7cwtvTdC4aAkBM6DiYh │
│   │            │       │                                              │ 9bpF"}                                        │
│ 1 │ video-key2 │ local │ pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f │ {"@type":"/cosmos.crypto.secp256k1.PubKey","k │
│   │            │       │                                              │ ey":"ArQDFUSK7jQpUPPNV35uxGGGz9j3cGNzOWvAVhG0 │
│   │            │       │                                              │ 0o9g"}                                        │
╰───┴────────────┴───────┴──────────────────────────────────────────────┴───────────────────────────────────────────────╯

❯ pussy keys list | from json | get address
╭───┬──────────────────────────────────────────────╮
│ 0 │ pussy12jlz63jwry4j3jshxlxwx6aulu6kssf83nsxm9 │
│ 1 │ pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f │
╰───┴──────────────────────────────────────────────╯

❯ pussy keys list | from json | get address.1
pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f

❯ pussy keys list
[{"name":"video-key","type":"local","address":"pussy12jlz63jwry4j3jshxlxwx6aulu6kssf83nsxm9","pubkey":"{\"@type\":\"/cosmos.crypto.secp256k1.PubKey\",\"key\":\"AlEs5WAVVDNyuBtPC00AI7cwtvTdC4aAkBM6DiYh9bpF\"}"},{"name":"video-key2","type":"local","address":"pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f","pubkey":"{\"@type\":\"/cosmos.crypto.secp256k1.PubKey\",\"key\":\"ArQDFUSK7jQpUPPNV35uxGGGz9j3cGNzOWvAVhG00o9g\"}"}]

❯ pussy keys list | from json
╭───┬────────────┬───────┬──────────────────────────────────────────────┬───────────────────────────────────────────────╮
│ # │    name    │ type  │                   address                    │                    pubkey                     │
├───┼────────────┼───────┼──────────────────────────────────────────────┼───────────────────────────────────────────────┤
│ 0 │ video-key  │ local │ pussy12jlz63jwry4j3jshxlxwx6aulu6kssf83nsxm9 │ {"@type":"/cosmos.crypto.secp256k1.PubKey","k │
│   │            │       │                                              │ ey":"AlEs5WAVVDNyuBtPC00AI7cwtvTdC4aAkBM6DiYh │
│   │            │       │                                              │ 9bpF"}                                        │
│ 1 │ video-key2 │ local │ pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f │ {"@type":"/cosmos.crypto.secp256k1.PubKey","k │
│   │            │       │                                              │ ey":"ArQDFUSK7jQpUPPNV35uxGGGz9j3cGNzOWvAVhG0 │
│   │            │       │                                              │ 0o9g"}                                        │
╰───┴────────────┴───────┴──────────────────────────────────────────────┴───────────────────────────────────────────────╯

❯ pussy keys list | from json | get address
╭───┬──────────────────────────────────────────────╮
│ 0 │ pussy12jlz63jwry4j3jshxlxwx6aulu6kssf83nsxm9 │
│ 1 │ pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f │
╰───┴──────────────────────────────────────────────╯

❯ pussy keys list | from json | get address.1
pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f

❯ let key1 = (pussy keys list | from json | get address.1)

❯ $key1
pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f

❯

❯ pussy query bank balances $key1
{"balances":[{"denom":"pussy","amount":"10000000000"}],"pagination":{"next_key":null,"total":"0"}}

❯ pussy query bank balances $key1
{"balances":[{"denom":"pussy","amount":"10000000000"}],"pagination":{"next_key":null,"total":"0"}}

❯ pussy query bank balances $key1 | from json
╭────────────┬───────────────────╮
│ balances   │ [table 1 row]     │
│ pagination │ {record 2 fields} │
╰────────────┴───────────────────╯

❯ pussy query bank balances $key1 | from json | get balances
╭───┬───────┬─────────────╮
│ # │ denom │   amount    │
├───┼───────┼─────────────┤
│ 0 │ pussy │ 10000000000 │
╰───┴───────┴─────────────╯

❯ pussy query bank balances $key1 | from json | get balances.amount.0
10000000000

❯ let amount1 = (pussy query bank balances $key1 | from json | get balances.amount.0)

❯ $amount1
10000000000

❯ let validators1 = (pussy query staking validators -o json | from json)

❯ $validators1
╭────────────┬───────────────────╮
│ validators │ [table 39 rows]   │
│ pagination │ {record 2 fields} │
╰────────────┴───────────────────╯

❯

❯ $validators1.validators
╭────┬──────────┬──────────┬────────┬──────────┬──────────┬──────────┬──────────┬─────────┬─────────┬─────────┬─────────╮
│  # │ operator │ consensu │ jailed │  status  │  tokens  │ delegato │ descript │ unbondi │ unbondi │ commiss │ min_sel │
│    │ _address │ s_pubkey │        │          │          │ r_shares │ ion      │ ng_heig │ ng_time │ ion     │ f_deleg │
│    │          │          │        │          │          │          │          │ ht      │         │         │ ation   │
├────┼──────────┼──────────┼────────┼──────────┼──────────┼──────────┼──────────┼─────────┼─────────┼─────────┼─────────┤
│  0 │ pussyval │ {record  │ false  │ BOND_STA │ 33104206 │ 33104206 │ {record  │ 0       │ 1970-01 │ {record │ 1000000 │
│    │ oper1p5s │ 2        │        │ TUS_BOND │ 8566496  │ 8566496. │ 5        │         │ -01T00: │  2      │ 000     │
│    │ udrdkr9r │ fields}  │        │ ED       │          │ 00000000 │ fields}  │         │ 00:00Z  │ fields} │         │
│    │ 8a84s7fh │          │        │          │          │ 00000000 │          │         │         │         │         │
│    │ 27tkhdrh │          │        │          │          │ 00       │          │         │         │         │         │
│    │ ujhqau8d │          │        │          │          │          │          │         │         │         │         │
│    │ u7t      │          │        │          │          │          │          │         │         │         │         │
│  1 │ pussyval │ {record  │ true   │ BOND_STA │ 99990000 │ 10000000 │ {record  │ 10001   │ 2022-11 │ {record │ 1000000 │
│    │ oper1p74 │ 2        │        │ TUS_UNBO │ 0000     │ 00000.00 │ 5        │         │ -01T12: │  2      │ 000     │
│    │ unan6vpp │ fields}  │        │ NDED     │          │ 00000000 │ fields}  │         │ 37:41.2 │ fields} │         │
│    │ 9frdcz2n │          │        │          │          │ 00000000 │          │         │ 2701772 │         │         │
│    │ hv8z59jx │          │        │          │          │          │          │         │ 0Z      │         │         │
│    │ 295nje80 │          │        │          │          │          │          │         │         │         │         │
│    │ wxd      │          │        │          │          │          │          │         │         │         │         │
│ 23 │ pussyval │ {record  │ false  │ BOND_STA │ 10912224 │ 10912224 │ {record  │ 0       │ 1970-01 │ {record │ 1000000 │
│    │ oper14hr │ 2        │        │ TUS_BOND │ 93779860 │ 93779860 │ 5        │         │ -01T00: │  2      │ 000     │
│    │ qklee0tx │ fields}  │        │ ED       │          │ .0000000 │ fields}  │         │ 00:00Z  │ fields} │         │
│    │ 6asycyfj │          │        │          │          │ 00000000 │          │         │         │         │         │
│    │ 357keql2 │          │        │          │          │ 000      │          │         │         │         │         │
│    │ jr5rdhq3 │          │        │          │          │          │          │         │         │         │         │
│    │ ytl      │          │        │          │          │          │          │         │         │         │         │
├────┼──────────┼──────────┼────────┼──────────┼──────────┼──────────┼──────────┼─────────┼─────────┼─────────┼─────────┤
│  # │ operator │ consensu │ jailed │  status  │  tokens  │ delegato │ descript │ unbondi │ unbondi │ commiss │ min_sel │
│    │ _address │ s_pubkey │        │          │          │ r_shares │ ion      │ ng_heig │ ng_time │ ion     │ f_deleg │
│    │          │          │        │          │          │          │          │ ht      │         │         │ ation   │
╰────┴──────────┴──────────┴────────┴──────────┴──────────┴──────────┴──────────┴─────────┴─────────┴─────────┴─────────╯

❯ $validators1.validators | flatten
╭────┬─────────┬─────────┬─────────┬────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────────┬─────╮
│  # │ operato │  @type  │   key   │ jailed │ status  │ tokens  │ delegat │ moniker │ identit │ website │ securit │ ... │
│    │ r_addre │         │         │        │         │         │ or_shar │         │ y       │         │ y_conta │     │
│    │ ss      │         │         │        │         │         │ es      │         │         │         │ ct      │     │
├────┼─────────┼─────────┼─────────┼────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────┤
│  0 │ pussyva │ /cosmos │ dfy2Tjb │ false  │ BOND_ST │ 3310420 │ 3310420 │ Bloqhub │         │         │         │ ... │
│    │ loper1p │ .crypto │ 24fytmL │        │ ATUS_BO │ 6856649 │ 6856649 │         │         │         │         │     │
│    │ 5sudrdk │ .ed2551 │ aTIqMRi │        │ NDED    │ 6       │ 6.00000 │         │         │         │         │     │
│    │ r9r8a84 │ 9.PubKe │ gVfwh7m │        │         │         │ 0000000 │         │         │         │         │     │
│    │ s7fh27t │ y       │ X4gr2C3 │        │         │         │ 000000  │         │         │         │         │     │
│    │ khdrhuj │         │ prhcBPd │        │         │         │         │         │         │         │         │     │
│    │ hqau8du │         │ 0=      │        │         │         │         │         │         │         │         │     │
│    │ 7t      │         │         │        │         │         │         │         │         │         │         │     │
│  1 │ pussyva │ /cosmos │ BMTtI0s │ true   │ BOND_ST │ 9999000 │ 1000000 │ Mimino  │         │         │         │ ... │
│    │ loper1p │ .crypto │ CeGPqmA │        │ ATUS_UN │ 00000   │ 000000. │         │         │         │         │     │
│    │ 74unan6 │ .ed2551 │ iKUsm4N │        │ BONDED  │         │ 0000000 │         │         │         │         │     │
│    │ vpp9frd │ 9.PubKe │ 7rstiKY │        │         │         │ 0000000 │         │         │         │         │     │
│    │ cz2nhv8 │ y       │ 6WFA1P2 │        │         │         │ 0000    │         │         │         │         │     │
│    │ z59jx29 │         │ Il9wD5E │        │         │         │         │         │         │         │         │     │
│    │ 5nje80w │         │ o=      │        │         │         │         │         │         │         │         │     │
│    │ xd      │         │         │        │         │         │         │         │         │         │         │     │
│ 23 │ pussyva │ /cosmos │ jSKJDVC │ false  │ BOND_ST │ 1091222 │ 1091222 │ Joy     │         │         │         │ ... │
│    │ loper14 │ .crypto │ /AGr6D+ │        │ ATUS_BO │ 4937798 │ 4937798 │ prophet │         │         │         │     │
│    │ hrqklee │ .ed2551 │ nnmdhMe │        │ NDED    │ 60      │ 60.0000 │         │         │         │         │     │
│    │ 0tx6asy │ 9.PubKe │ +zmPinq │        │         │         │ 0000000 │         │         │         │         │     │
│    │ cyfj357 │ y       │ rEMSlSs │        │         │         │ 0000000 │         │         │         │         │     │
│    │ keql2jr │         │ Yja0FB7 │        │         │         │         │         │         │         │         │     │
│    │ 5rdhq3y │         │ w=      │        │         │         │         │         │         │         │         │     │
│    │ tl      │         │         │        │         │         │         │         │         │         │         │     │
├────┼─────────┼─────────┼─────────┼────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────────┼─────┤
│  # │ operato │  @type  │   key   │ jailed │ status  │ tokens  │ delegat │ moniker │ identit │ website │ securit │ ... │
│    │ r_addre │         │         │        │         │         │ or_shar │         │ y       │         │ y_conta │     │
│    │ ss      │         │         │        │         │         │ es      │         │         │         │ ct      │     │
╰────┴─────────┴─────────┴─────────┴────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────────┴─────╯

❯ $validators1.validators | flatten | select operator_address moniker
╭────┬─────────────────────────────────────────────────────┬──────────────────────────────────────────╮
│  # │                  operator_address                   │                 moniker                  │
├────┼─────────────────────────────────────────────────────┼──────────────────────────────────────────┤
│  0 │ pussyvaloper1p5sudrdkr9r8a84s7fh27tkhdrhujhqau8du7t │ Bloqhub                                  │
│  1 │ pussyvaloper1p74unan6vpp9frdcz2nhv8z59jx295nje80wxd │ Mimino                                   │
│  2 │ pussyvaloper1zaefvwrgk2g45k68a3ngahgq0xky5zge60rqhp │ POSTCAPITALIST🎩                         │
│  3 │ pussyvaloper1rxdzc0c80u9wympy8sgmx32ra0df5dzt322tc4 │ MikeLitoris                              │
│  4 │ pussyvaloper1r8d26xgfxr80v3slu8r6z7wkl4h7f99q2s3z72 │ web34ever                                │
│  5 │ pussyvaloper1r28nhrkwcvqs4qss2l7zqdvc2qfdl8ardvna7m │ PoorButHappy                             │
│  6 │ pussyvaloper1r7q209q5yeh9d37pftdsm2eqtrl45ry8g79u8f │ Papsan                                   │
│  7 │ pussyvaloper19yyulmnkzwyuq9tzfhy4vdvftp0dsdvc9gw2q3 │ 777stakes                                │
│  8 │ pussyvaloper1xq8lgu7n3f9yagd7qmd5vegva6j56plnryy6cw │ Tokyo                                    │
│  9 │ pussyvaloper1xehfjcpw7nddd7s5xpyzkqvft99saqqv6j69jt │ Galaxy                                   │
│ 10 │ pussyvaloper1gwlqmqc9nrnuu8fanls76exyrzum9xjm6weada │ BigfOOT                                  │
│ 11 │ pussyvaloper12kpw3e9ypjal6upmju9smwgjhwefpt7vc4azgf │ Stigga                                   │
│ 12 │ pussyvaloper1vg8lh3dsp7023kz79mlk642dux9vu038k78q9l │ ToTheMars                                │
│ 13 │ pussyvaloper1v46pz6ddetfc3tnvdr28ss0l48jhazgyw9ef94 │ linak                                    │
│ 14 │ pussyvaloper1wm4026rxqcrkh09k806m6y4lys942etxf326cf │ PLap                                     │
│ 15 │ pussyvaloper10trdf5eyfcmc9graltx4hmpgznhrm7hdlwjwhc │ goto5k                                   │
│ 16 │ pussyvaloper10jmsqhf7mwquv0wa08hegxqaasvue5tnymgxq8 │ cccatch                                  │
│ 17 │ pussyvaloper13pff76ycsnsuh8z3kssmcjazs3e29s66dx53gv │ StakeLabz                                │
│ 18 │ pussyvaloper13jnp8uk4xnqcvdejcnq9rphm9actc90p709qgl │ inch88                                   │
│ 19 │ pussyvaloper135ca8hdpy9sk0ntwqzpzsvatyl48ptx50cvazf │ cyberdBot                                │
│ 20 │ pussyvaloper1j3w0aa7s6665puyls9lwx9ej6cz2afystpfeed │ Bro_n_Bro                                │
│ 21 │ pussyvaloper1n8hu3cqsn3txf0ltdk3x0sff2s0yt96xnv0h0e │ Denwer                                   │
│ 22 │ pussyvaloper14fwr9m4rf27r3txv5luvph98nrckyu2qpvkx3t │ ChainManiacs | Real Solar&Wind validator │
│ 23 │ pussyvaloper14hrqklee0tx6asycyfj357keql2jr5rdhq3ytl │ Joy prophet                              │
│ 24 │ pussyvaloper1kfqme88c6vq8mt0smw29z67k4zz2ykr6p7jkx5 │ space                                    │
│ 25 │ pussyvaloper1ke3aflev7cr75gxa54k6qwrajfc53vqhzp08vd │ PensionFund4ALL                          │
│ 26 │ pussyvaloper1hyrtrdqnayvvtznddczjymjcj2jagcqulv8laa │ Developer                                │
│ 27 │ pussyvaloper1h4pfcqsykh53a8k5sup6nq78v5shjlfje600na │ Apollo                                   │
│ 28 │ pussyvaloper1cwu6g93hnfm44zyl8cnkn58dsakxh2aczqajxn │ roksax                                   │
│ 29 │ pussyvaloper1csq8phy88f4js7fml6zzt454lr2py2c3spsdun │ Godzilla                                 │
│ 30 │ pussyvaloper1ezqvp6aga74ms7jqrfwhrm7266sn2m502v2gl2 │ AlphaCentavra                            │
│ 31 │ pussyvaloper1ezpth4mp3eeqdt49kgqd5ctr69xev6v24dwepg │ csaxial                                  │
│ 32 │ pussyvaloper1e8238v24qccht9mqc2w0r4luq462yxtt9h2plz │ POSTHUMAN ꝏ DVS                          │
│ 33 │ pussyvaloper1m0tjgkrh4td9fcp8nnssu3rfdahzfgds2e98zw │ lux8.net                                 │
│ 34 │ pussyvaloper1m5rf5fvhrl76s3xkvh3kde0p4dpwzewu5a3s5j │ KURASH                                   │
│ 35 │ pussyvaloper1uynj0jhl059u9t5h4ug9075jrepdz4cw24av7l │ Citizen Cosmos                           │
│ 36 │ pussyvaloper1u2kvnwxmmpru764l5ht3nxkfwwu6ytw485yhwp │ Kerman                                   │
│ 37 │ pussyvaloper17zdyl3gfssc3vzzyxptnr0xl8z0pnte92zy8vy │ cyberG                                   │
│ 38 │ pussyvaloper17rh7gz9f8w7klw2nvtdj2v85zrdapvzhsp5t2g │ Mercury                                  │
├────┼─────────────────────────────────────────────────────┼──────────────────────────────────────────┤
│  # │                  operator_address                   │                 moniker                  │
╰────┴─────────────────────────────────────────────────────┴──────────────────────────────────────────╯

❯ $validators1.validators | flatten | select operator_address moniker | where moniker == "Joy prophet"
╭───┬─────────────────────────────────────────────────────┬─────────────╮
│ # │                  operator_address                   │   moniker   │
├───┼─────────────────────────────────────────────────────┼─────────────┤
│ 0 │ pussyvaloper14hrqklee0tx6asycyfj357keql2jr5rdhq3ytl │ Joy prophet │
╰───┴─────────────────────────────────────────────────────┴─────────────╯

❯ $validators1.validators | flatten | select operator_address moniker | where moniker == "Joy prophet" | get operator_address
╭───┬─────────────────────────────────────────────────────╮
│ 0 │ pussyvaloper14hrqklee0tx6asycyfj357keql2jr5rdhq3ytl │
╰───┴─────────────────────────────────────────────────────╯

❯ $validators1.validators | flatten | select operator_address moniker | where moniker == "Joy prophet" | get operator_address.0
pussyvaloper14hrqklee0tx6asycyfj357keql2jr5rdhq3ytl

❯ let validator1 = ($validators1.validators | flatten | select operator_address moniker | where moniker == "Joy prophet" | get operator_address.0)

❯

❯ pussy tx staking delegate -h
Delegate an amount of liquid coins to a validator from your wallet.

Example:
$ spacepussy tx staking delegate pussyvaloper1l2rsakp388kuv9k8qzq6lrm9taddae7fpx59wm 1000stake --from mykey

Usage:
  pussy tx staking delegate [validator-addr] [amount] [flags]

Flags:
  -a, --account-number uint      The account number of the signing account (offline mode only)
  -b, --broadcast-mode string    Transaction broadcasting mode (sync|async|block) (default "sync")
      --dry-run                  ignore the --gas flag and perform a simulation of a transaction, but don't broadcast it
      --fee-account string       Fee account pays fees for the transaction instead of deducting from the signer
      --fees string              Fees to pay along with transaction; eg: 10uatom
      --from string              Name or address of private key with which to sign
      --gas string               gas limit to set per-transaction; set to "auto" to calculate sufficient gas automatically (default 200000)
      --gas-adjustment float     adjustment factor to be multiplied against the estimate returned by the tx simulation; if the gas limit is set manually this flag is ignored  (default 1)
      --gas-prices string        Gas prices in decimal format to determine the transaction fee (e.g. 0.1uatom)
      --generate-only            Build an unsigned transaction and write it to STDOUT (when enabled, the local Keybase is not accessible)
  -h, --help                     help for delegate
      --keyring-backend string   Select keyring's backend (os|file|kwallet|pass|test|memory) (default "os")
      --keyring-dir string       The client Keyring directory; if omitted, the default 'home' directory will be used
      --ledger                   Use a connected Ledger device
      --node string              <host>:<port> to tendermint rpc interface for this chain (default "tcp://localhost:26657")
      --note string              Note to add a description to the transaction (previously --memo)
      --offline                  Offline mode (does not allow any online functionality
  -o, --output string            Output format (text|json) (default "json")
  -s, --sequence uint            The sequence number of the signing account (offline mode only)
      --sign-mode string         Choose sign mode (direct|amino-json), this is an advanced feature
      --timeout-height uint      Set a block timeout height to prevent the tx from being committed past a certain height
  -y, --yes                      Skip tx broadcasting prompt confirmation

Global Flags:
      --chain-id string     The network chain ID
      --home string         directory for config and data (default "/Users/uuser/.pussy")
      --log_format string   The logging format (json|plain) (default "plain")
      --log_level string    The logging level (trace|debug|info|warn|error|fatal|panic) (default "info")
      --trace               print out full stack trace on errors

❯

❯ $amount1
10000000000

❯ $amount1 | into int
10000000000

❯ $amount1 | into int | $in * 0.98
9800000000

❯ $amount1 | into int | $in * 0.98 | into string
9800000000

❯ $amount1 | into int | $in * 0.98 | into string | $in + 'pussy'
9800000000pussy

❯ ( $amount1 | into int ) * 0.98
9800000000

❯ let amount_pussy = ($amount1 | into int | $in * 0.98 | into string | $in + 'pussy')

❯ pussy tx staking delegate -h
Delegate an amount of liquid coins to a validator from your wallet.

Example:
$ spacepussy tx staking delegate pussyvaloper1l2rsakp388kuv9k8qzq6lrm9taddae7fpx59wm 1000stake --from mykey

Usage:
  pussy tx staking delegate [validator-addr] [amount] [flags]

Flags:
  -a, --account-number uint      The account number of the signing account (offline mode only)
  -b, --broadcast-mode string    Transaction broadcasting mode (sync|async|block) (default "sync")
      --dry-run                  ignore the --gas flag and perform a simulation of a transaction, but don't broadcast it
      --fee-account string       Fee account pays fees for the transaction instead of deducting from the signer
      --fees string              Fees to pay along with transaction; eg: 10uatom
      --from string              Name or address of private key with which to sign
      --gas string               gas limit to set per-transaction; set to "auto" to calculate sufficient gas automatically (default 200000)
      --gas-adjustment float     adjustment factor to be multiplied against the estimate returned by the tx simulation; if the gas limit is set manually this flag is ignored  (default 1)
      --gas-prices string        Gas prices in decimal format to determine the transaction fee (e.g. 0.1uatom)
      --generate-only            Build an unsigned transaction and write it to STDOUT (when enabled, the local Keybase is not accessible)
  -h, --help                     help for delegate
      --keyring-backend string   Select keyring's backend (os|file|kwallet|pass|test|memory) (default "os")
      --keyring-dir string       The client Keyring directory; if omitted, the default 'home' directory will be used
      --ledger                   Use a connected Ledger device
      --node string              <host>:<port> to tendermint rpc interface for this chain (default "tcp://localhost:26657")
      --note string              Note to add a description to the transaction (previously --memo)
      --offline                  Offline mode (does not allow any online functionality
  -o, --output string            Output format (text|json) (default "json")
  -s, --sequence uint            The sequence number of the signing account (offline mode only)
      --sign-mode string         Choose sign mode (direct|amino-json), this is an advanced feature
      --timeout-height uint      Set a block timeout height to prevent the tx from being committed past a certain height
  -y, --yes                      Skip tx broadcasting prompt confirmation

Global Flags:
      --chain-id string     The network chain ID
      --home string         directory for config and data (default "/Users/uuser/.pussy")
      --log_format string   The logging format (json|plain) (default "plain")
      --log_level string    The logging level (trace|debug|info|warn|error|fatal|panic) (default "info")
      --trace               print out full stack trace on errors

❯ pussy tx staking delegate $validator1 $amount_pussy --from video-key2
{"body":{"messages":[{"@type":"/cosmos.staking.v1beta1.MsgDelegate","delegator_address":"pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f","validator_address":"pussyvaloper14hrqklee0tx6asycyfj357keql2jr5rdhq3ytl","amount":{"denom":"pussy","amount":"9800000000"}}],"memo":"","timeout_height":"0","extension_options":[],"non_critical_extension_options":[]},"auth_info":{"signer_infos":[],"fee":{"amount":[],"gas_limit":"200000","payer":"","granter":""}},"signatures":[]}

confirm transaction before signing and broadcasting [y/N]: y
{"height":"0","txhash":"827F2F144449836A8A8F746EAA904831239D2F10F4B3BAFF4332FAC8F4B52161","codespace":"","code":0,"data":"","raw_log":"[]","logs":[],"info":"","gas_wanted":"0","gas_used":"0","tx":null,"timestamp":"","events":[]}
 took 5s
❯ pussy query bank balances $key1
{"balances":[{"denom":"liquidpussy","amount":"9800000000"},{"denom":"pussy","amount":"200000000"}],"pagination":{"next_key":null,"total":"0"}}

❯ let balance2 = (pussy query bank balances $key1 | from json)

❯ $balance2
╭────────────┬───────────────────╮
│ balances   │ [table 2 rows]    │
│ pagination │ {record 2 fields} │
╰────────────┴───────────────────╯

❯ $balance2.balances
╭───┬─────────────┬────────────╮
│ # │    denom    │   amount   │
├───┼─────────────┼────────────┤
│ 0 │ liquidpussy │ 9800000000 │
│ 1 │ pussy       │ 200000000  │
╰───┴─────────────┴────────────╯

❯ $balance2.balances | where denom == 'liquidpussy'
╭───┬─────────────┬────────────╮
│ # │    denom    │   amount   │
├───┼─────────────┼────────────┤
│ 0 │ liquidpussy │ 9800000000 │
╰───┴─────────────┴────────────╯

❯ $balance2.balances | where denom == 'liquidpussy' | get amount.0
9800000000

❯ let balance_liquid = ($balance2.balances | where denom == 'liquidpussy' | get amount.0)

❯ $balance_liquid
9800000000

❯ 24*60*60*30
Error: nu::shell::external_command (link)

  × External command failed
   ╭─[entry #55:1:1]
 1 │ 24*60*60*30
   · ─────┬─────
   ·      ╰── executable was not found
   ╰────
  help: No such file or directory (os error 2)


❯ 24 * 60 * 60 * 30
2592000

❯ pussy tx resources investmint $"($balance_liquid * 0.8)liquidpussy" millivolt 2592000 --from video-key2
Error: nu::shell::type_mismatch (link)

  × Type mismatch during operation.
   ╭─[entry #57:1:1]
 1 │ pussy tx resources investmint $"($balance_liquid * 0.8)liquidpussy" millivolt 2592000 --from video-key2
   ·                                  ───────┬─────── ┬ ─┬─
   ·                                         │        │  ╰── float
   ·                                         │        ╰── type mismatch for operator
   ·                                         ╰── string
   ╰────


❯ pussy tx resources investmint $"(($balance_liquid | into int) * 0.8)liquidpussy" millivolt 2592000 --from video-key2

{"body":{"messages":[{"@type":"/cyber.resources.v1beta1.MsgInvestmint","neuron":"pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f","amount":{"denom":"liquidpussy","amount":"7840000000"},"resource":"millivolt","length":"2592000"}],"memo":"","timeout_height":"0","extension_options":[],"non_critical_extension_options":[]},"auth_info":{"signer_infos":[],"fee":{"amount":[],"gas_limit":"200000","payer":"","granter":""}},"signatures":[]}

confirm transaction before signing and broadcasting [y/N]: cancelled transaction

❯ pussy tx resources investmint $"(($balance_liquid | into int) * 0.8)liquidpussy" millivolt 2592000 --from video-key2
{"body":{"messages":[{"@type":"/cyber.resources.v1beta1.MsgInvestmint","neuron":"pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f","amount":{"denom":"liquidpussy","amount":"7840000000"},"resource":"millivolt","length":"2592000"}],"memo":"","timeout_height":"0","extension_options":[],"non_critical_extension_options":[]},"auth_info":{"signer_infos":[],"fee":{"amount":[],"gas_limit":"200000","payer":"","granter":""}},"signatures":[]}

confirm transaction before signing and broadcasting [y/N]: y
{"height":"0","txhash":"6FB50A5E02FB2A14406CDB1C6A334E43810DEABC7581524212AE0EB35F42C071","codespace":"","code":0,"data":"","raw_log":"[]","logs":[],"info":"","gas_wanted":"0","gas_used":"0","tx":null,"timestamp":"","events":[]}
 took 3s
❯ pussy tx resources investmint $"(($balance_liquid | into int) * 0.2)liquidpussy" milliampere 2592000 --from video-key2
{"body":{"messages":[{"@type":"/cyber.resources.v1beta1.MsgInvestmint","neuron":"pussy1stp7rvpl2sr0vnzyw3l7yhflllk4ueux2ynr9f","amount":{"denom":"liquidpussy","amount":"1960000000"},"resource":"milliampere","length":"2592000"}],"memo":"","timeout_height":"0","extension_options":[],"non_critical_extension_options":[]},"auth_info":{"signer_infos":[],"fee":{"amount":[],"gas_limit":"200000","payer":"","granter":""}},"signatures":[]}

confirm transaction before signing and broadcasting [y/N]: y
{"height":"0","txhash":"16C2C2E7B58A79ED28C660666F6CB9D5FE26E45760F5FE84066E0D5B7CEDF434","codespace":"","code":0,"data":"","raw_log":"[]","logs":[],"info":"","gas_wanted":"0","gas_used":"0","tx":null,"timestamp":"","events":[]}
 took 3s
❯
```
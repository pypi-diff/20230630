# Comparing `tmp/dexie_rewards-1.8.1b2.tar.gz` & `tmp/dexie_rewards-1.8.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexie_rewards-1.8.1b2.tar", max compression
+gzip compressed data, was "dexie_rewards-1.8.2b1.tar", max compression
```

## Comparing `dexie_rewards-1.8.1b2.tar` & `dexie_rewards-1.8.2b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-30 14:18:44.184005 dexie_rewards-1.8.1b2/LICENSE
--rw-r--r--   0        0        0     5716 2023-06-11 05:14:21.000000 dexie_rewards-1.8.1b2/README.md
--rw-r--r--   0        0        0      800 2023-06-11 05:36:33.383744 dexie_rewards-1.8.1b2/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-04 04:23:21.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/__init__.py
--rw-r--r--   0        0        0     1125 2023-06-10 08:56:40.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/config.py
--rw-r--r--   0        0        0      822 2023-05-12 12:18:23.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/decorators/with_db_connection.py
--rw-r--r--   0        0        0     1169 2023-06-10 08:56:40.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/decorators/with_wallet_rpc_client.py
--rw-r--r--   0        0        0      234 2023-05-08 10:51:08.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/main.py
--rw-r--r--   0        0        0     4557 2023-06-10 08:56:40.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/claim.py
--rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/list.py
--rw-r--r--   0        0        0      272 2023-05-08 10:18:31.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/main.py
--rw-r--r--   0        0        0     5043 2023-06-11 05:27:12.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/utils.py
--rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/services/dexie_api.py
--rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/services/dexie_db.py
--rw-r--r--   0        0        0     1792 2023-06-11 05:27:12.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/services/wallet_rpc_client.py
--rw-r--r--   0        0        0      801 2023-05-16 00:41:08.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/types/offer_reward.py
--rw-r--r--   0        0        0      229 2023-05-09 11:06:14.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/types/utils.py
--rw-r--r--   0        0        0     1863 2023-06-10 08:56:40.000000 dexie_rewards-1.8.1b2/src/dexie_rewards/utils.py
--rw-r--r--   0        0        0     6547 1970-01-01 00:00:00.000000 dexie_rewards-1.8.1b2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-1.8.2b1/LICENSE
+-rw-r--r--   0        0        0     5721 2023-06-11 09:31:39.287155 dexie_rewards-1.8.2b1/README.md
+-rw-r--r--   0        0        0      805 2023-06-30 09:11:11.103550 dexie_rewards-1.8.2b1/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-1.8.2b1/src/dexie_rewards/__init__.py
+-rw-r--r--   0        0        0     1125 2023-06-30 04:40:39.340510 dexie_rewards-1.8.2b1/src/dexie_rewards/config.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-1.8.2b1/src/dexie_rewards/decorators/with_db_connection.py
+-rw-r--r--   0        0        0     1169 2023-06-10 08:56:40.443038 dexie_rewards-1.8.2b1/src/dexie_rewards/decorators/with_wallet_rpc_client.py
+-rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-1.8.2b1/src/dexie_rewards/main.py
+-rw-r--r--   0        0        0     5013 2023-06-30 09:40:10.161232 dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/claim.py
+-rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/list.py
+-rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/main.py
+-rw-r--r--   0        0        0     5159 2023-06-30 09:37:14.115364 dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/utils.py
+-rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.341294 dexie_rewards-1.8.2b1/src/dexie_rewards/services/dexie_api.py
+-rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-1.8.2b1/src/dexie_rewards/services/dexie_db.py
+-rw-r--r--   0        0        0     1792 2023-06-11 05:27:12.034750 dexie_rewards-1.8.2b1/src/dexie_rewards/services/wallet_rpc_client.py
+-rw-r--r--   0        0        0     1124 2023-06-30 04:32:23.576365 dexie_rewards-1.8.2b1/src/dexie_rewards/types/offer_reward.py
+-rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-1.8.2b1/src/dexie_rewards/types/utils.py
+-rw-r--r--   0        0        0     1863 2023-06-10 08:56:40.444913 dexie_rewards-1.8.2b1/src/dexie_rewards/utils.py
+-rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 dexie_rewards-1.8.2b1/PKG-INFO
```

### Comparing `dexie_rewards-1.8.1b2/LICENSE` & `dexie_rewards-1.8.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b2/README.md` & `dexie_rewards-1.8.2b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Auto-Claim dexie rewards
 
 [![PyPI version](https://badge.fury.io/py/dexie-rewards.svg)](https://badge.fury.io/py/dexie-rewards)
 [![Python version](https://img.shields.io/pypi/pyversions/dexie-rewards.svg)](https://pypi.python.org/pypi/dexie-rewards)
 
-dexie-rewards is a Python CLI helper tool designed automatically claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
+dexie-rewards is a Python CLI helper tool designed to automatically claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
 
 When rewards are claimed, a message from the input (maker) address of the offer is signed to prove ownership of the offer. The signature is then sent to dexie to claim the rewards. dexie distributes claimed rewards to the input (maker) address in batches approximately every 15 minutes.
 
 ## Example Output
 
 ```
 ❯ dexie rewards claim
@@ -30,14 +30,15 @@
 It is recommended to install dexie-rewards using pip.
 
 ### Install via pip
 
 ```sh
 pip install dexie-rewards
 ```
+
 Note for macOS: If `pip` is not found, try `pip3` instead.
 
 ### Install from the repository (optional)
 
 1. Clone the repository
 
 ```sh
@@ -71,32 +72,34 @@
 ## Available Commands
 
 Make sure that your Chia wallet is running and fully synced before using dexie-rewards. A full node is not required.
 
 Run any command with the `--help` option to see all available functionality.
 
 ### List offers with outstanding (claimable) rewards
+
 ```
 ❯ dexie rewards list
 
   --fingerprint  -f        Set the fingerprint to specify which wallet to use
   --json         -j        Displays offers as JSON
   --verbose      -v        Display verbose output
   --help                   Show help and exit
 ```
 
 ### Claim all outstanding (claimable) rewards
+
 ```
 ❯ dexie rewards claim
 
   --fingerprint  -f         Set the fingerprint to specify which wallet to use
   --verify-only  -vo        Only verify the claim, don't actually claim
   --yes          -y         Skip claim confirmation
   --verbose      -v         Display verbose output
-  --target       -t         Specify a target address to claim rewards to 
+  --target       -t         Specify a target address to claim rewards to
   --help                    Show help and exit
 ```
 
 ## Troubleshooting
 
 If you encounter any issues, follow these steps to help identify and resolve them:
```

### Comparing `dexie_rewards-1.8.1b2/pyproject.toml` & `dexie_rewards-1.8.2b1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "dexie-rewards"
-version = "1.8.1-b2"
+version = "1.8.2-b1"
 description = "dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "dexie_rewards", from = "src" }]
 
 [tool.poetry.dependencies]
-python = ">=3.10"
+python = ">=3.10,<4.0"
 rich-click = "^1.6.1"
 aiomisc = "^17.0.9"
 aiohttp = "^3.8.4"
 based58 = "^0.1.1"
 chia-blockchain = "1.8.*"
-aiosqlite = "^0.17.0"
+aiosqlite = "^0.19.0"
 
 [tool.poetry.scripts]
 dexie = "dexie_rewards.main:dexie_cmd"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 mypy = "^1.2.0"
```

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/config.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/config.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/decorators/with_db_connection.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/decorators/with_db_connection.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/decorators/with_wallet_rpc_client.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/decorators/with_wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/claim.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/claim.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,53 +74,75 @@
     "-t",
     "--target",
     "target_puzzle_hash",
     help="Specify a target address to claim rewards to",
     type=ChiaWalletAddressParamType(),
     required=False,
 )
+@click.option(
+    "-co",
+    "--completed-only",
+    help="Only claim rewards for completed and cancelled offers",
+    is_flag=True,
+    default=False,
+    show_default=True,
+)
 def claim_cmds(
     fingerprint: Optional[int],
     verify_only: bool,
     skip_confirm: bool,
     verbose: bool,
     target_puzzle_hash: Optional[bytes32],
+    completed_only: bool,
 ) -> None:
     asyncio.run(
         claim_cmds_async(
-            fingerprint, verify_only, skip_confirm, verbose, target_puzzle_hash
+            fingerprint,
+            verify_only,
+            skip_confirm,
+            verbose,
+            target_puzzle_hash,
+            completed_only,
         )
     )
 
 
 async def claim_cmds_async(
     fingerprint: Optional[int],
     verify_only: bool,
     skip_confirm: bool,
     verbose: bool,
     target_puzzle_hash: Optional[bytes32],
+    completed_only: bool,
 ) -> None:
     try:
         console = Console(file=StringIO()) if not verbose else Console()
 
         synced_fingerprint = await wait_for_synced_wallet(fingerprint)
         await dexie_db.create_db(synced_fingerprint)
 
         offers_rewards_dict = await get_offers_with_claimable_rewards(
             synced_fingerprint, console
         )
-        offers_rewards = list(map(OfferReward.from_json_dict, offers_rewards_dict))
+
+        offers_rewards = list(
+            filter(
+                (lambda o: not o.is_active) if completed_only else (lambda _: True),
+                map(OfferReward.from_json_dict, offers_rewards_dict),
+            )
+        )
+
         if len(offers_rewards) == 0:
             console.print("No rewards to claim", style="bold red")
             return
 
         display_rewards(offers_rewards)
 
         if not skip_confirm:
-            if not Confirm.ask("Claim all?"):
+            if not Confirm.ask(f"Claim all?"):
                 return
 
         claims = await create_claims(offers_rewards, target_puzzle_hash)
         ret: Any = {"claims": claims}
         if target_puzzle_hash is not None:
             ret["target_puzzle_hash"] = target_puzzle_hash.hex()
```

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/list.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/list.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/rewards/utils.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/rewards/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,19 @@
 
 async def create_claims(
     offers_rewards: List[OfferReward], target_puzzle_hash: Optional[bytes32]
 ) -> List[Any]:
     timestamp = int(time.time())
     claims = []
     for offer_reward in offers_rewards:
-        (public_key, signature, signing_mode,) = await sign_claim(
+        (
+            public_key,
+            signature,
+            signing_mode,
+        ) = await sign_claim(
             offer_reward.offer_id,
             timestamp,
             offer_reward.maker_puzzle_hash,
             target_puzzle_hash,
         )
 
         # return offer hash, signature, pk, and puzzle hash
@@ -139,15 +143,17 @@
         "Rewards (DBX)",
         justify="right",
         footer=Text(f"{total_rewards}"),
     )
 
     for offer_reward in offers_rewards:
         offer_hash = Text(offer_reward.offer_id)
-        offer_hash.stylize(f"bold {dexie_blue}")
+        offer_hash.stylize(
+            f"{dexie_blue} {'strike' if not offer_reward.is_active else 'bold'}"
+        )
         offer_hash.stylize(f"link {dexie_url}/offers/{offer_reward.offer_id}")
         amount = "{0:0.3f}".format(offer_reward.claimable_rewards)
         table.add_row(
             offer_hash,
             amount,
         )
```

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/services/dexie_api.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/services/dexie_api.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/services/dexie_db.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/services/dexie_db.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/services/wallet_rpc_client.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/services/wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/types/offer_reward.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/types/offer_reward.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,7 +20,16 @@
         return cls(
             offer_id=json_dict["id"],
             is_active=True if json_dict["status"] == 0 else False,
             claimable_rewards=round(float(json_dict["claimable_rewards"]), 3),
             date_found=to_datetime(json_dict["date_found"]),
             maker_puzzle_hash=bytes32.from_hexstr(json_dict["maker_puzzle_hash"]),
         )
+
+    def to_json_dict(self) -> Dict[str, Any]:
+        return {
+            "id": self.offer_id,
+            "is_active": self.is_active,
+            "claimable_rewards": self.claimable_rewards,
+            "date_found": self.date_found.isoformat(),
+            "maker_puzzle_hash": self.maker_puzzle_hash.hex(),
+        }
```

### Comparing `dexie_rewards-1.8.1b2/src/dexie_rewards/utils.py` & `dexie_rewards-1.8.2b1/src/dexie_rewards/utils.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-1.8.1b2/PKG-INFO` & `dexie_rewards-1.8.2b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: dexie-rewards
-Version: 1.8.1b2
+Version: 1.8.2b1
 Summary: dexie-rewards is a Python CLI helper tool designed automatically to claim dexie liquidity rewards for offers created using the official Chia Wallet.
 License: Apache-2.0
 Author: Dexie Contributors
 Author-email: pypi@dexie.space
-Requires-Python: >=3.10
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aiomisc (>=17.0.9,<18.0.0)
-Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
+Requires-Dist: aiosqlite (>=0.19.0,<0.20.0)
 Requires-Dist: based58 (>=0.1.1,<0.2.0)
-Requires-Dist: chia-blockchain (>=1.8.0,<1.9.0)
+Requires-Dist: chia-blockchain (==1.8.*)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Auto-Claim dexie rewards
 
 [![PyPI version](https://badge.fury.io/py/dexie-rewards.svg)](https://badge.fury.io/py/dexie-rewards)
 [![Python version](https://img.shields.io/pypi/pyversions/dexie-rewards.svg)](https://pypi.python.org/pypi/dexie-rewards)
 
-dexie-rewards is a Python CLI helper tool designed automatically claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
+dexie-rewards is a Python CLI helper tool designed to automatically claim [dexie liquidity rewards](https://dexie.space/incentives) for offers created using the official Chia Wallet. The tool communicates locally with the Chia Wallet RPC, requests all created offers, and checks them for claimable rewards.
 
 When rewards are claimed, a message from the input (maker) address of the offer is signed to prove ownership of the offer. The signature is then sent to dexie to claim the rewards. dexie distributes claimed rewards to the input (maker) address in batches approximately every 15 minutes.
 
 ## Example Output
 
 ```
 ❯ dexie rewards claim
@@ -50,14 +50,15 @@
 It is recommended to install dexie-rewards using pip.
 
 ### Install via pip
 
 ```sh
 pip install dexie-rewards
 ```
+
 Note for macOS: If `pip` is not found, try `pip3` instead.
 
 ### Install from the repository (optional)
 
 1. Clone the repository
 
 ```sh
@@ -91,32 +92,34 @@
 ## Available Commands
 
 Make sure that your Chia wallet is running and fully synced before using dexie-rewards. A full node is not required.
 
 Run any command with the `--help` option to see all available functionality.
 
 ### List offers with outstanding (claimable) rewards
+
 ```
 ❯ dexie rewards list
 
   --fingerprint  -f        Set the fingerprint to specify which wallet to use
   --json         -j        Displays offers as JSON
   --verbose      -v        Display verbose output
   --help                   Show help and exit
 ```
 
 ### Claim all outstanding (claimable) rewards
+
 ```
 ❯ dexie rewards claim
 
   --fingerprint  -f         Set the fingerprint to specify which wallet to use
   --verify-only  -vo        Only verify the claim, don't actually claim
   --yes          -y         Skip claim confirmation
   --verbose      -v         Display verbose output
-  --target       -t         Specify a target address to claim rewards to 
+  --target       -t         Specify a target address to claim rewards to
   --help                    Show help and exit
 ```
 
 ## Troubleshooting
 
 If you encounter any issues, follow these steps to help identify and resolve them:
```


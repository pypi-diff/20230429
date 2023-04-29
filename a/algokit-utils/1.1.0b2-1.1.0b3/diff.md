# Comparing `tmp/algokit_utils-1.1.0b2-py3-none-any.whl.zip` & `tmp/algokit_utils-1.1.0b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 32456 bytes, number of entries: 14
--rw-r--r--  2.0 unx     3767 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
--rw-r--r--  2.0 unx     7366 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
--rw-r--r--  2.0 unx     7709 b- defN 80-Jan-01 00:00 algokit_utils/account.py
+Zip file size: 33086 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     3697 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
+-rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
+-rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
+-rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    53906 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    29956 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     3930 b- defN 80-Jan-01 00:00 algokit_utils/models.py
--rw-r--r--  2.0 unx     5065 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
+-rw-r--r--  2.0 unx     4841 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1175 b- defN 16-Jan-01 00:00 algokit_utils-1.1.0b2.dist-info/RECORD
-14 files, 125522 bytes uncompressed, 30502 bytes compressed:  75.7%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.1.0b3.dist-info/RECORD
+15 files, 125584 bytes uncompressed, 30994 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: algokit_utils/__init__.py
 Comment: 
 
+Filename: algokit_utils/_ensure_funded.py
+Comment: 
+
 Filename: algokit_utils/_transfer.py
 Comment: 
 
 Filename: algokit_utils/account.py
 Comment: 
 
 Filename: algokit_utils/application_client.py
@@ -24,20 +27,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.1.0b2.dist-info/LICENSE
+Filename: algokit_utils-1.1.0b3.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.1.0b2.dist-info/METADATA
+Filename: algokit_utils-1.1.0b3.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.1.0b2.dist-info/WHEEL
+Filename: algokit_utils-1.1.0b3.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.1.0b2.dist-info/RECORD
+Filename: algokit_utils-1.1.0b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/__init__.py

```diff
@@ -1,22 +1,20 @@
+from algokit_utils._ensure_funded import EnsureBalanceParameters, ensure_funded
 from algokit_utils._transfer import (
-    EnsureBalanceParameters,
     TransferParameters,
-    ensure_funded,
     transfer,
 )
 from algokit_utils.account import (
     create_kmd_wallet_account,
     get_account,
     get_account_from_mnemonic,
     get_dispenser_account,
     get_kmd_wallet_account,
     get_localnet_default_account,
     get_or_create_kmd_wallet_account,
-    get_sandbox_default_account,
 )
 from algokit_utils.application_client import (
     ApplicationClient,
     Program,
     execute_atc_with_logic_error,
     get_next_version,
     get_sender_from_signer,
@@ -74,23 +72,21 @@
     get_algod_client,
     get_algonode_config,
     get_default_localnet_config,
     get_indexer_client,
     get_kmd_client_from_algod_client,
     get_purestake_config,
     is_localnet,
-    is_sandbox,
 )
 
 __all__ = [
     "create_kmd_wallet_account",
     "get_account_from_mnemonic",
     "get_or_create_kmd_wallet_account",
     "get_localnet_default_account",
-    "get_sandbox_default_account",
     "get_dispenser_account",
     "get_kmd_wallet_account",
     "get_account",
     "UPDATABLE_TEMPLATE_NAME",
     "DELETABLE_TEMPLATE_NAME",
     "NOTE_PREFIX",
     "DeploymentFailedError",
@@ -141,13 +137,12 @@
     "get_algod_client",
     "get_algonode_config",
     "get_default_localnet_config",
     "get_indexer_client",
     "get_kmd_client_from_algod_client",
     "get_purestake_config",
     "is_localnet",
-    "is_sandbox",
     "EnsureBalanceParameters",
     "TransferParameters",
     "ensure_funded",
     "transfer",
 ]
```

## algokit_utils/_transfer.py

```diff
@@ -8,15 +8,15 @@
 from algosdk.transaction import PaymentTxn, SuggestedParams
 
 from algokit_utils.models import Account
 
 if TYPE_CHECKING:
     from algosdk.v2client.algod import AlgodClient
 
-__all__ = ["EnsureBalanceParameters", "TransferParameters", "ensure_funded", "transfer"]
+__all__ = ["TransferParameters", "transfer"]
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass(kw_only=True)
 class TransferParameters:
     """Parameters for transferring µALGOs between accounts"""
 
@@ -29,47 +29,15 @@
     suggested_params: SuggestedParams | None = None
     """(optional) transaction parameters"""
     note: str | bytes | None = None
     """(optional) transaction note"""
     fee_micro_algos: int | None = None
     """(optional) The flat fee you want to pay, useful for covering extra fees in a transaction group or app call"""
     max_fee_micro_algos: int | None = None
-    """(optional)The maximum fee that you are happy to pay (default: unbounded) -
-    if this is set it's possible the transaction could get rejected during network congestion"""
-
-
-@dataclasses.dataclass(kw_only=True)
-class EnsureBalanceParameters:
-    """Parameters for ensuring an account has a minimum number of µALGOs"""
-
-    account_to_fund: Account | AccountTransactionSigner | str
-    """The account address that will receive the µALGOs"""
-
-    funding_source: Account | AccountTransactionSigner
-    """The account (with private key) or signer that will send the µALGOs"""
-
-    min_spending_balance_micro_algos: int
-    """The minimum balance of ALGOs that the account should have available to spend (i.e. on top of
-    minimum balance requirement)"""
-
-    min_funding_increment_micro_algos: int = 0
-    """When issuing a funding amount, the minimum amount to transfer (avoids many small transfers if this gets
-    called often on an active account)"""
-
-    suggested_params: SuggestedParams | None = None
-    """(optional) transaction parameters"""
-
-    note: str | bytes | None = None
-    """The (optional) transaction note, default: "Funding account to meet minimum requirement"""
-
-    fee_micro_algos: int | None = None
-    """(optional) The flat fee you want to pay, useful for covering extra fees in a transaction group or app call"""
-
-    max_fee_micro_algos: int | None = None
-    """(optional)The maximum fee that you are happy to pay (default: unbounded) -
+    """(optional) The maximum fee that you are happy to pay (default: unbounded) -
     if this is set it's possible the transaction could get rejected during network congestion"""
 
 
 def _check_fee(transaction: PaymentTxn, max_fee: int | None) -> None:
     if max_fee is not None:
         # Once a transaction has been constructed by algosdk, transaction.fee indicates what the total transaction fee
         # Will be based on the current suggested fee-per-byte value.
@@ -110,55 +78,7 @@
     txid = transaction.get_txid()  # type: ignore[no-untyped-call]
     logger.debug(
         f"Sent transaction {txid} type={transaction.type} from "
         f"{address_from_private_key(from_account.private_key)}"  # type: ignore[no-untyped-call]
     )
 
     return transaction
-
-
-def ensure_funded(
-    client: "AlgodClient",
-    parameters: EnsureBalanceParameters,
-) -> None | PaymentTxn:
-    """
-    Funds a given account using a funding source such that it has a certain amount of algos free to spend
-    (accounting for ALGOs locked in minimum balance requirement)
-    see <https://developer.algorand.org/docs/get-details/accounts/#minimum-balance>
-
-    :return None | PaymentTxn: None if balance was sufficient or the payment transaction used to increase the balance
-    """
-    sender_address = address_from_private_key(parameters.funding_source.private_key)  # type: ignore[no-untyped-call]
-    address_to_fund = (
-        parameters.account_to_fund
-        if isinstance(parameters.account_to_fund, str)
-        else address_from_private_key(parameters.account_to_fund.private_key)  # type: ignore[no-untyped-call]
-    )
-
-    account_info = client.account_info(address_to_fund)
-    assert isinstance(account_info, dict)
-
-    balance_micro_algos = account_info.get("amount", 0)
-    minimum_balance_micro_algos = account_info.get("min-balance")
-    current_spending_balance_micro_algos = balance_micro_algos - minimum_balance_micro_algos
-    if parameters.min_spending_balance_micro_algos > current_spending_balance_micro_algos:
-        min_fund_amount_micro_algos = parameters.min_spending_balance_micro_algos - current_spending_balance_micro_algos
-        fund_amount_micro_algos = max(min_fund_amount_micro_algos, parameters.min_funding_increment_micro_algos)
-        logger.info(
-            f"Funding {address_to_fund} {fund_amount_micro_algos}µ from {sender_address} to reach "
-            f"minimum spend amount of {parameters.min_spending_balance_micro_algos}µ (balance = "
-            f"{balance_micro_algos}µ, requirement = {minimum_balance_micro_algos}µ)"
-        )
-        return transfer(
-            client,
-            TransferParameters(
-                from_account=parameters.funding_source,
-                to_address=address_to_fund,
-                micro_algos=fund_amount_micro_algos,
-                note=parameters.note or "Funding account to meet minimum requirement",
-                suggested_params=parameters.suggested_params,
-                max_fee_micro_algos=parameters.max_fee_micro_algos,
-                fee_micro_algos=parameters.fee_micro_algos,
-            ),
-        )
-
-    return None
```

## algokit_utils/account.py

```diff
@@ -1,10 +1,9 @@
 import logging
 import os
-import warnings
 from typing import TYPE_CHECKING, Any
 
 from algosdk.account import address_from_private_key
 from algosdk.mnemonic import from_private_key, to_private_key
 from algosdk.util import algos_to_microalgos
 
 from algokit_utils._transfer import TransferParameters, transfer
@@ -21,15 +20,14 @@
     "create_kmd_wallet_account",
     "get_account",
     "get_account_from_mnemonic",
     "get_dispenser_account",
     "get_kmd_wallet_account",
     "get_localnet_default_account",
     "get_or_create_kmd_wallet_account",
-    "get_sandbox_default_account",
 ]
 
 logger = logging.getLogger(__name__)
 _DEFAULT_ACCOUNT_MINIMUM_BALANCE = 1_000_000_000
 
 
 def get_account_from_mnemonic(mnemonic: str) -> Account:
@@ -88,23 +86,14 @@
     return account
 
 
 def _is_default_account(account: dict[str, Any]) -> bool:
     return bool(account["status"] != "Offline" and account["amount"] > _DEFAULT_ACCOUNT_MINIMUM_BALANCE)
 
 
-def get_sandbox_default_account(client: "AlgodClient") -> Account:
-    warnings.warn(
-        "get_sandbox_default_account is deprecated, please use get_localnet_default_account instead",
-        DeprecationWarning,
-        stacklevel=2,
-    )
-    return get_localnet_default_account(client)
-
-
 def get_localnet_default_account(client: "AlgodClient") -> Account:
     """Returns the default Account in a LocalNet instance"""
     if not is_localnet(client):
         raise Exception("Can't get a default account from non LocalNet network")
 
     account = get_kmd_wallet_account(
         client, get_kmd_client_from_algod_client(client), "unencrypted-default-wallet", _is_default_account
```

## algokit_utils/network_clients.py

```diff
@@ -1,10 +1,9 @@
 import dataclasses
 import os
-import warnings
 from typing import Literal
 from urllib import parse
 
 from algosdk.kmd import KMDClient
 from algosdk.v2client.algod import AlgodClient
 from algosdk.v2client.indexer import IndexerClient
 
@@ -13,15 +12,14 @@
     "get_algod_client",
     "get_algonode_config",
     "get_default_localnet_config",
     "get_indexer_client",
     "get_kmd_client_from_algod_client",
     "get_purestake_config",
     "is_localnet",
-    "is_sandbox",
 ]
 
 _PURE_STAKE_HOST = "purestake.io"
 
 
 @dataclasses.dataclass
 class AlgoClientConfig:
@@ -80,19 +78,14 @@
 
 def is_localnet(client: AlgodClient) -> bool:
     """Returns True if client genesis is `devnet-v1` or `sandnet-v1`"""
     params = client.suggested_params()
     return params.gen in ["devnet-v1", "sandnet-v1"]
 
 
-def is_sandbox(client: AlgodClient) -> bool:
-    warnings.warn("is_sandbox is deprecated, please use is_localnet instead", DeprecationWarning, stacklevel=2)
-    return is_localnet(client)
-
-
 def get_kmd_client_from_algod_client(client: AlgodClient) -> KMDClient:
     """Returns an {py:class}`algosdk.kmd.KMDClient` from supplied `client`
 
     Will use the same address as provided `client` but on port specified by `KMD_PORT` environment variable,
     or 4002 by default"""
     # We can only use Kmd on the LocalNet otherwise it's not exposed so this makes some assumptions
     # (e.g. same token and server as algod and port 4002 by default)
```

## Comparing `algokit_utils-1.1.0b2.dist-info/LICENSE` & `algokit_utils-1.1.0b3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.1.0b2.dist-info/METADATA` & `algokit_utils-1.1.0b3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.1.0b2
+Version: 1.1.0b3
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


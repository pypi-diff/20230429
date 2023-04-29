# Comparing `tmp/pyarmor.cli-8.1.dev9-py2.py3-none-any.whl.zip` & `tmp/pyarmor.cli-8.2.dev1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 33129 bytes, number of entries: 18
--rw-r--r--  2.0 unx     1292 b- defN 23-Apr-05 16:02 pyarmor/cli/__init__.py
--rw-r--r--  2.0 unx    20090 b- defN 23-Apr-08 23:41 pyarmor/cli/__main__.py
--rw-r--r--  2.0 unx     8608 b- defN 23-Apr-02 14:49 pyarmor/cli/config.py
--rw-r--r--  2.0 unx    15562 b- defN 23-Apr-08 00:25 pyarmor/cli/context.py
--rw-r--r--  2.0 unx     7736 b- defN 23-Apr-08 04:34 pyarmor/cli/default.cfg
--rw-r--r--  2.0 unx      880 b- defN 23-Jan-12 09:29 pyarmor/cli/errors.py
--rw-r--r--  2.0 unx     5603 b- defN 23-Apr-05 01:07 pyarmor/cli/generate.py
--rw-r--r--  2.0 unx     4008 b- defN 23-Feb-11 01:53 pyarmor/cli/mixer.py
+Zip file size: 36451 bytes, number of entries: 18
+-rw-r--r--  2.0 unx     1479 b- defN 23-Apr-25 01:18 pyarmor/cli/__init__.py
+-rw-r--r--  2.0 unx    22591 b- defN 23-Apr-28 23:46 pyarmor/cli/__main__.py
+-rw-r--r--  2.0 unx    10694 b- defN 23-Apr-20 07:01 pyarmor/cli/config.py
+-rw-r--r--  2.0 unx    17255 b- defN 23-Apr-28 22:34 pyarmor/cli/context.py
+-rw-r--r--  2.0 unx     7475 b- defN 23-Apr-27 00:20 pyarmor/cli/default.cfg
+-rw-r--r--  2.0 unx     5553 b- defN 23-Apr-22 00:21 pyarmor/cli/generate.py
+-rw-r--r--  2.0 unx     3956 b- defN 23-Apr-20 07:02 pyarmor/cli/mixer.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Apr-22 14:15 pyarmor/cli/plugin.py
 -rw-r--r--  2.0 unx     2487 b- defN 23-Mar-25 22:51 pyarmor/cli/public_capsule.zip
--rw-r--r--  2.0 unx    10980 b- defN 23-Apr-06 22:19 pyarmor/cli/register.py
--rw-r--r--  2.0 unx    11386 b- defN 23-Mar-29 13:18 pyarmor/cli/repack.py
--rw-r--r--  2.0 unx     6366 b- defN 23-Apr-06 11:59 pyarmor/cli/resource.py
+-rw-r--r--  2.0 unx    17413 b- defN 23-Apr-29 00:43 pyarmor/cli/register.py
+-rw-r--r--  2.0 unx    11386 b- defN 23-Apr-20 07:01 pyarmor/cli/repack.py
+-rw-r--r--  2.0 unx     6398 b- defN 23-Apr-13 06:46 pyarmor/cli/resource.py
 -rw-r--r--  2.0 unx     2193 b- defN 23-Feb-22 14:43 pyarmor/cli/shell.py
--rw-r--r--  2.0 unx     2405 b- defN 23-Apr-08 23:42 pyarmor.cli-8.1.dev9.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-08 23:42 pyarmor.cli-8.1.dev9.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 23-Apr-08 23:42 pyarmor.cli-8.1.dev9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-08 23:42 pyarmor.cli-8.1.dev9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1465 b- defN 23-Apr-08 23:42 pyarmor.cli-8.1.dev9.dist-info/RECORD
-18 files, 101220 bytes uncompressed, 30747 bytes compressed:  69.6%
+-rw-r--r--  2.0 unx     2407 b- defN 23-Apr-29 01:11 pyarmor.cli-8.2.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-29 01:11 pyarmor.cli-8.2.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Apr-29 01:11 pyarmor.cli-8.2.dev1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 01:11 pyarmor.cli-8.2.dev1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1467 b- defN 23-Apr-29 01:11 pyarmor.cli-8.2.dev1.dist-info/RECORD
+18 files, 115760 bytes uncompressed, 34069 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pyarmor/cli/context.py
 Comment: 
 
 Filename: pyarmor/cli/default.cfg
 Comment: 
 
-Filename: pyarmor/cli/errors.py
-Comment: 
-
 Filename: pyarmor/cli/generate.py
 Comment: 
 
 Filename: pyarmor/cli/mixer.py
 Comment: 
 
+Filename: pyarmor/cli/plugin.py
+Comment: 
+
 Filename: pyarmor/cli/public_capsule.zip
 Comment: 
 
 Filename: pyarmor/cli/register.py
 Comment: 
 
 Filename: pyarmor/cli/repack.py
@@ -33,23 +33,23 @@
 
 Filename: pyarmor/cli/resource.py
 Comment: 
 
 Filename: pyarmor/cli/shell.py
 Comment: 
 
-Filename: pyarmor.cli-8.1.dev9.dist-info/METADATA
+Filename: pyarmor.cli-8.2.dev1.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli-8.1.dev9.dist-info/WHEEL
+Filename: pyarmor.cli-8.2.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli-8.1.dev9.dist-info/entry_points.txt
+Filename: pyarmor.cli-8.2.dev1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pyarmor.cli-8.1.dev9.dist-info/top_level.txt
+Filename: pyarmor.cli-8.2.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli-8.1.dev9.dist-info/RECORD
+Filename: pyarmor.cli-8.2.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/__init__.py

```diff
@@ -1,11 +1,17 @@
 import logging
 
 __VERSION__ = '8.1'
 
+logger = logging.getLogger('cli')
+
+
+class CliError(Exception):
+    pass
+
 
 def resoptions(meth):
 
     def process(self, res, *args, **kwargs):
         self._options = self.ctx.get_res_options(res.fullname, self._Catalog)
         return meth(self, res, *args, **kwargs)
 
@@ -14,33 +20,37 @@
 
 class Component(object):
 
     trace_loggers = {
         'StrProtector': 'trace.mix.str',
         'CallProtector': 'trace.assert.call',
         'ImportProtector': 'trace.assert.import',
+        'CodeProtector': 'trace.co',
         'CoPatcher': 'trace.co',
         'BccPatcher': 'trace.bcc',
     }
 
     def __init__(self, ctx):
         self.ctx = ctx
         self._options = {}
 
         clsname = self.__class__.__name__
         self.logger = logging.getLogger(self.trace_loggers[clsname])
 
     def __getattr__(self, opt):
         if opt.startswith('o_'):
-            return self._options.get(opt[2:])
+            return self._options.get(opt[2:], '')
         elif opt.startswith('oi_'):
             return int(self._options.get(opt[3:]))
         elif opt.startswith('ob_'):
             v = self._options.get(opt[3:], '')
             if isinstance(v, str):
+                if v.isdigit():
+                    return bool(int(v))
                 return v.lower() in ('1', 'true', 'on', 'yes')
+
             return v
         return AttributeError(opt)
 
     def trace(self, res, node, value):
         lineno = getattr(node, 'lineno', -1)
         self.logger.info('%s:%s:%s', res.fullname, lineno, value)
```

## pyarmor/cli/__main__.py

```diff
@@ -20,44 +20,49 @@
 #  @Create Date: Thu Jan 12 10:27:05 CST 2023
 #
 import argparse
 import logging
 import os
 import sys
 
-from .errors import CliError
+from . import logger, CliError
 from .context import Context
 from .register import Register, WebRegister
 from .config import Configer
 from .shell import PyarmorShell
-
-logger = logging.getLogger('Pyarmor')
+from .plugin import Plugin
 
 
 def _cmd_gen_key(builder, options):
     n = len(options['inputs'])
     if n > 1:
-        raise CliError('too many args %s' % options['inputs'][1:])
+        logger.error('please check online documentation to learn')
+        logger.error('how to use command "pyarmor gen key"')
+        raise CliError('invalid arguments: %s' % options['inputs'][1:])
     keyname = builder.ctx.outer_keyname
 
     logger.info('start to generate outer runtime key "%s"', keyname)
     data = builder.generate_runtime_key(outer=True)
     output = options.get('output', 'dist')
     os.makedirs(output, exist_ok=True)
 
     target = os.path.join(output, keyname)
     logger.info('write %s', target)
     with open(target, 'wb') as f:
         f.write(data)
+
+    Plugin.post_key(builder.ctx, target)
     logger.info('generate outer runtime key OK')
 
 
 def _cmd_gen_runtime(builder, options):
     if len(options['inputs']) > 1:
-        raise CliError('too many args %s' % options['inputs'][1:])
+        logger.error('please check online documentation to learn')
+        logger.error('how to use command "pyarmor gen runtime"')
+        raise CliError('invalid arguments: %s' % options['inputs'][1:])
 
     output = options.get('output', 'dist')
 
     logger.info('start to generate runtime package')
     builder.generate_runtime(output)
 
     keyname = os.path.join(output, builder.ctx.runtime_keyfile)
@@ -74,14 +79,25 @@
               'obf_module', 'obf_code', 'assert_import', 'assert_call',
               'mix_str', 'import_prefix', 'restrict_module',
               'platforms', 'outer', 'period', 'expired', 'devices'):
         v = getattr(args, x)
         if v is not None:
             options[x] = v
 
+    if options.get('platforms'):
+        platforms = []
+        for item in options['platforms']:
+            platforms.extend([x.strip() for x in item.split(',')])
+        options['platforms'] = platforms
+    elif ctx.runtime_platforms:
+        options['platforms'] = ctx.runtime_platforms.split()
+        logger.info('get runtime platforms from configuration file')
+    if options.get('platforms'):
+        logger.info('use runtime platforms: %s', options['platforms'])
+
     if args.inputs:
         options['inputs'] = [os.path.normpath(x) for x in args.inputs]
 
     if args.use_runtime:
         options['no_runtime'] = True
         options['use_runtime'] = args.use_runtime
 
@@ -92,44 +108,58 @@
 
     if options.get('restrict_module', 0) > 1:
         options['mix_coname'] = 1
 
     if args.enables:
         for x in args.enables:
             options['enable_' + x] = True
+    if options.get('enable_themida'):
+        raise NotImplementedError('--enable_themida is still not implemented')
 
     if args.prefix:
         options['import_prefix'] = args.prefix
 
     if args.no_wrap:
         options['wrap_mode'] = 0
 
     if args.includes:
         options['includes'] = ' '.join(args.includes)
     if args.excludes:
         options['excludes'] = ' '.join(args.excludes)
 
+    if args.bind_data:
+        options['user_data'] = args.bind_data
+
     return options
 
 
 def check_cross_platform(ctx, platforms):
+    rtver = ctx.cfg.get('pyarmor', 'cli.runtime')
+    cmd = 'pip install pyarmor.cli.runtime~=%s.0' % rtver
     try:
         from pyarmor.cli import runtime
-    except ModuleNotFoundError:
-        raise CliError('cross platform need pyarmor.cli.runtime, please '
-                       'run "pip install pyarmor.cli.runtime==2.1.dev9" first')
+    except (ImportError, ModuleNotFoundError):
+        logger.error('cross platform need package "pyarmor.cli.runtime"')
+        logger.error('please run "%s" to fix it', cmd)
+        raise CliError('no package "pyarmor.cli.runtime" found')
+
+    if runtime.__VERSION__ != rtver:
+        logger.error('please run "%s" to fix it', cmd)
+        raise CliError('unexpected "pyarmor.cli.runtime" version')
 
     platnames = []
     for path in runtime.__path__:
+        logger.debug('search runtime platforms at: %s', path)
         platnames.extend(os.listdir(os.path.join(path, 'libs')))
 
     map_platform = runtime.map_platform
     unknown = set([map_platform(x) for x in platforms]) - set(platnames)
 
     if unknown:
+        logger.error('please check documentation "References/Environments"')
         raise CliError('unsupported platforms "%s"' % ', '.join(unknown))
 
 
 def check_gen_context(ctx, args):
     enable_bcc = args.enable_bcc or (args.enables and 'bcc' in args.enables)
     if ctx.runtime_platforms:
         if ctx.enable_themida and not ctx.pyarmor_platform.startswith('win'):
@@ -140,47 +170,53 @@
 
     if enable_bcc:
         plat, arch = ctx.pyarmor_platform.split('.')
         if arch not in ('x86_64', 'aarch64'):
             raise CliError('bcc mode still not support arch "%s"' % arch)
 
     if ctx.cmd_options['no_runtime'] and not ctx.runtime_outer:
-        raise CliError('--no_runtime need pass outer key by --outer')
+        raise CliError('--no_runtime must be used with --outer')
 
     if ctx.use_runtime and not ctx.runtime_outer:
         if os.path.exists(ctx.use_runtime):
             keyname = os.path.join(ctx.use_runtime, ctx.runtime_keyfile)
             if not os.path.exists(keyname):
                 raise CliError('no runtime key in "%s"', ctx.use_runtime)
 
     if ctx.runtime_outer and any(
             [ctx.runtime_devices, ctx.runtime_period, ctx.runtime_expired]):
         raise CliError('--outer conflicts with any -e, --period, -b')
 
-    if args.pack and (args.no_runtime or ctx.import_prefix):
-        raise CliError('--pack conficts with --no-runtime, --use-runtime, '
-                       '-i, --prefix')
+    if args.pack:
+        if not os.path.isfile(args.pack):
+            raise CliError('--pack must be an executable file')
+        if args.no_runtime:
+            raise CliError('--pack conficts with --no-runtime, --use-runtime')
+        if ctx.import_prefix:
+            raise CliError('--pack conficts with -i, --prefix')
 
 
 def cmd_gen(ctx, args):
     from .generate import Builder
 
     options = format_gen_args(ctx, args)
     logger.debug('command options: %s', options)
     ctx.push(options)
     check_gen_context(ctx, args)
 
     builder = Builder(ctx)
 
+    Plugin.install(ctx)
     if args.inputs[0].lower() in ('key', 'k'):
         _cmd_gen_key(builder, options)
     elif args.inputs[0].lower() in ('runtime', 'run', 'r'):
         _cmd_gen_runtime(builder, options)
     else:
         builder.process(options, pack=args.pack)
+        Plugin.post_build(ctx, pack=args.pack)
 
 
 def cmd_cfg(ctx, args):
     scope = 'global' if args.scope else 'local'
     cfg = Configer(ctx, encoding=args.encoding)
     name = 'reset' if args.reset else 'run'
     getattr(cfg, name)(args.options, scope == 'local', args.name)
@@ -188,68 +224,84 @@
 
 def cmd_reg(ctx, args):
     if args.buy:
         from webbrowser import open_new_tab
         open_new_tab(ctx.cfg['pyarmor']['buyurl'])
         return
 
+    if args.device and not args.regfile:
+        reg = Register(ctx)
+        reg.generate_group_device(args.device)
+        logger.info('device file has been generated successfully')
+        return
+
     regfile = args.regfile
     if not regfile:
         reg = Register(ctx)
         logger.info('Current license information:\n\n%s', reg)
         return
 
+    if regfile.endswith('.txt') and not args.product:
+        logger.error('please use -p to specify product name for this license')
+        raise CliError('missing product name')
+
+    if regfile.endswith('.zip') and args.product:
+        logger.error('please do not use -p for non initial registration')
+        raise CliError('unwanted product name')
+
     upgrade = args.upgrade
     if upgrade:
         if not regfile.endswith('.txt'):
             raise CliError('upgrade need text file "pyarmor-keycode-xxxx.txt"')
         url = 'https://github.com/dashingsoft/pyarmor/issues/980'
         msg = ("",
-               "Pyarmor 8.0 changes EULA and uses new commands",
+               "Pyarmor 8 changes EULA and uses new commands",
                "It's different from previous Pyarmor totally",
                "Please read this import notes first:",
                url,
-               "Do not upgrade to Pyarmor 8 if you don't known what's changed",
+               "Do not upgrade to Pyarmor 8 if don't know what are changed",
                "", "")
         prompt = 'I have known the changes of Pyarmor 8? (yes/no/help) '
         choice = input('\n'.join(msg) + prompt).lower()[:1]
         if choice == 'h':
             import webbrowser
             webbrowser.open(url)
         if not choice == 'y':
             return
 
-    if regfile.endswith('.zip'):
+    if args.device:
+        if not regfile.endswith('.zip'):
+            logger.error('invalid registeration file "%s"', regfile)
+            raise CliError('please use ".zip" file to register group device')
+        regsvr = WebRegister(ctx)
+        regsvr.register_group_device(regfile, args.device)
+        logger.info('The device regfile has been generated successfully')
+
+    elif regfile.endswith('.zip'):
         reg = Register(ctx)
         logger.info('register "%s"', regfile)
         reg.register_regfile(regfile)
         logger.info('This license registration information:\n\n%s', str(reg))
 
     else:
         regsvr = WebRegister(ctx)
-        if (not args.confirm) or upgrade:
-            info, msg = regsvr.prepare(regfile, args.product, upgrade=upgrade)
-            prompt = 'Are you sure to continue? (yes/no) '
-            if input(msg + prompt) != 'yes':
-                return
-            if info['upgrade'] and info['product'] in ('TBD', 'non-profits'):
-                msg = '\n'.join([
-                    '',
-                    'The product name is set to "%s", once upgrade, '
-                    'it can not be changed.' % info['product'],
-                    ''
-                ])
-                if input(msg + prompt) != 'yes':
-                    return
-            # Free upgrade to Pyarmor Basic
-            if upgrade and not info['upgrade']:
-                return regsvr.register(regfile, args.product, upgrade=True)
-
-        meth = 'upgrade_to_pro' if upgrade else 'register'
-        getattr(regsvr, meth)(regfile, args.product)
+        info, msg = regsvr.prepare(regfile, args.product, upgrade=upgrade)
+        prompt = 'Are you sure to continue? (yes/no) '
+        if input(msg + prompt) not in ('y', 'yes'):
+            logger.info('abort registration')
+            return
+        # Free upgrade to Pyarmor Basic
+        if upgrade and not info['upgrade']:
+            return regsvr.register(regfile, args.product, upgrade=True)
+
+        if upgrade:
+            regsvr.upgrade_to_pro(regfile, args.product)
+        else:
+            group = info['lictype'] == 'GROUP'
+            regsvr.register(regfile, args.product, group=group)
 
 
 def main_parser():
     parser = argparse.ArgumentParser(
         prog='pyarmor',
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
@@ -287,15 +339,19 @@
     '''generate obfuscated scripts and all required runtime files
     pyarmor gen <options> <scripts>
 
 generate runtime key only
     pyarmor gen key <options>
 
 generate runtime package only
-    pyarmor gen runtime <options>'''
+    pyarmor gen runtime <options>
+
+Refer to
+https://pyarmor.readthedocs.io/en/stable/reference/man.html#pyarmor-gen
+'''
     cparser = subparsers.add_parser(
         'gen',
         aliases=['generate', 'g'],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=gen_parser.__doc__,
         help='generate obfuscated scripts and required runtime files'
     )
@@ -422,14 +478,18 @@
         help='check runtime key periodically'
     )
     group.add_argument(
         '-b', '--bind-device', dest='devices', metavar='DEV', action='append',
         help='bind obfuscated scripts to device'
     )
     group.add_argument(
+        '--bind-data', metavar='FILE',
+        help=argparse.SUPPRESS
+    )
+    group.add_argument(
         '--bind-interp', metavar='INTERP',
         help=argparse.SUPPRESS
     )
     group.add_argument(
         '--hook', metavar='HOOK',
         help=argparse.SUPPRESS
     )
@@ -447,14 +507,17 @@
     pyarmor cfg
 
 show option `OPT` value:
     pyarmor cfg OPT
 
 change option value:
     pyarmor cfg OPT=VALUE
+
+Refer to
+https://pyarmor.readthedocs.io/en/stable/reference/man.html#pyarmor-cfg
     '''
 
     cparser = subparsers.add_parser(
         'cfg',
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=cfg_parser.__doc__,
         help='show and config Pyarmor environments',
@@ -488,22 +551,19 @@
     cparser.set_defaults(func=cmd_cfg)
 
 
 def reg_parser(subparsers):
     '''register Pyarmor or upgrade Pyarmor license
 
 At the first time to register Pyarmor, `-p` (product name) should be
-set. If not set, this Pyarmor license is bind to "non-profits", and
-could not be used for commercial product.
-
-Once register successfully, product name can't be changed.
-
-There is only one exception, if product name is set to "TBD" at the
-first time, it can be changed once later.
+set. For non-commercial use, set it to "non-profits". The product name
+can't be changed after initial registration.
 
+Refer to
+https://pyarmor.readthedocs.io/en/stable/reference/man.html#pyarmor-reg
     '''
     cparser = subparsers.add_parser(
         'reg',
         aliases=['register', 'r'],
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=reg_parser.__doc__,
         help='register Pyarmor or upgrade Pyarmor license'
@@ -511,27 +571,31 @@
 
     cparser.add_argument(
         '-r', '--regname', metavar='NAME',
         help=argparse.SUPPRESS
     )
     cparser.add_argument(
         '-p', '--product', metavar='NAME',
-        help='license to this product'
+        help='bind license to this product'
     )
     cparser.add_argument(
         '-u', '--upgrade', action='store_true',
-        help='upgrade Pyarmor license'
+        help='upgrade old Pyarmor license'
+    )
+    cparser.add_argument(
+        '-g', '--device', metavar='ID', type=int, choices=range(1, 101),
+        help='device id (1-100) in group license'
     )
     cparser.add_argument(
         '--buy', action='store_true',
         help='open buy link in default web browser'
     )
     cparser.add_argument(
         '-y', '--confirm', action='store_true',
-        help='register Pyarmor without asking for confirmation'
+        help=argparse.SUPPRESS
     )
 
     cparser.add_argument(
         'regfile', nargs='?', metavar='FILE',
         help='pyarmor-regcode-xxx.txt or pyarmor-regfile-xxxx.zip'
     )
     cparser.set_defaults(func=cmd_reg)
@@ -556,19 +620,19 @@
         tracelog.addHandler(handler)
 
     if args.silent:
         logging.getLogger().setLevel(100)
 
 
 def log_exception(e):
-    logger.critical('unknown error, please check pyarmor.error.log')
+    logger.debug('unknown error, please check pyarmor.error.log')
     handler = logging.FileHandler('pyarmor.error.log', mode='w')
     fmt = '%(process)d %(processName)s %(asctime)s'
     handler.setFormatter(logging.Formatter(fmt))
-    log = logging.getLogger('Pyarmor.Error')
+    log = logging.getLogger('error')
     log.propagate = False
     log.addHandler(logging.NullHandler())
     log.addHandler(handler)
     log.exception(e)
 
 
 def print_version(ctx):
@@ -602,15 +666,15 @@
         parser.exit()
 
     if args.interactive:
         return PyarmorShell(ctx).cmdloop()
 
     logger.info('Python %d.%d.%d', *sys.version_info[:3])
     logger.info('Pyarmor %s', ctx.version_info())
-    logger.debug('Platform %s', ctx.pyarmor_platform)
+    logger.info('Platform %s', ctx.pyarmor_platform)
 
     logger.debug('native platform %s', ctx.native_platform)
     logger.debug('home path: %s', ctx.home_path)
 
     if hasattr(args, 'func'):
         args.func(ctx, args)
     else:
@@ -621,18 +685,17 @@
     logging.basicConfig(
         level=logging.INFO,
         format='%(levelname)-8s %(message)s',
     )
 
     try:
         main_entry(sys.argv[1:])
-    # # TBD: comment for debug
-    # except (CliError, RuntimeError) as e:
-    #     logger.error(e)
-    #     sys.exit(1)
+    except CliError as e:
+        logger.error(e)
+        sys.exit(1)
     except Exception as e:
         log_exception(e)
         logger.error(e)
         sys.exit(2)
 
 
 if __name__ == '__main__':
```

## pyarmor/cli/config.py

```diff
@@ -17,33 +17,33 @@
 #
 #  @Author: Jondy Zhao (pyarmor@163.com)
 #
 #  @Create Date: Thu Jan 12 10:27:05 CST 2023
 #
 import configparser
 import fnmatch
-import logging
 import os
 
-logger = logging.getLogger('Pyarmor')
+from . import logger, CliError
 
 
 def indent(lines, n=2):
     fmt = ' ' * 2 + '%s'
     return [fmt % x for x in lines]
 
 
 def str_opt(k, v, n=30):
+    v = '\n\t'.join(v.splitlines())
     return '  %s = %s%s' % (k, v[:n], '...' if len(v) > n else '')
 
 
 class Configer(object):
 
-    SECTIONS = 'pyarmor', 'logging', 'finder', 'builder', \
-        'pack', 'bcc', 'rft', 'mix.str', 'assert.call', 'assert.import'
+    SECTIONS = 'pyarmor', 'logging', 'finder', 'builder', 'runtime', \
+        'pack', 'bcc', 'mix.str', 'assert.call', 'assert.import'
 
     def __init__(self, ctx, encoding=None):
         self.ctx = ctx
         self._encoding = encoding
 
     def _read_config(self, filename):
         cfg = configparser.ConfigParser(empty_lines_in_values=False)
@@ -122,29 +122,47 @@
         if name:
             cfg = self._read_config(self.ctx.get_filename(local, name))
             if cfg.has_section(sect) and cfg.has_option(sect, opt):
                 plines.append(format_value(opt))
 
         return clines, glines, lines, plines
 
-    def _set_option(self, sect, opt, local=True, name=None):
+    def _set_option(self, sect, opt, value, local=True, name=None):
         ctx = self.ctx
         filename = ctx.get_filename(local=local, name=name)
 
         cfg = self._read_config(filename)
         if not cfg.has_section(sect):
             cfg.add_section(sect)
 
         # TBD: input multiple lines
-        optname, optvalue = opt.split('=', 2)
-        if optvalue and optvalue[0] in ("'", '"'):
+        optname, optvalue = opt, value
+        if optvalue and optvalue[:1] in ('+', '-', '=', '^'):
+            op = optvalue[:1]
+            optvalue = optvalue.strip(op)
+            if op == '=':
+                op = None
+        else:
+            op = None
+        if optvalue and optvalue[:1] in ("'", '"'):
             optvalue = optvalue.strip(optvalue[0])
 
         if not optvalue:
-            return self.clear(sect, optname, local, name)
+            if op is None:
+                self._clear(sect, optname, local, name)
+            return
+
+        old = cfg[sect].get(optname, '') if cfg.has_section(sect) else ''
+        if op == '+':
+            if (optvalue + ' ').find(old + ' ') == -1:
+                optvalue = ('%s %s' % (old, optvalue)).strip()
+        elif op == '-':
+            optvalue = (old + ' ').replace(optvalue + ' ', '').strip()
+        elif op == '^':
+            optvalue = '\n'.join((old.splitlines() + [optvalue]))
 
         logger.info('change option "%s" to new value "%s"', optname, optvalue)
         cfg.set(sect, optname, optvalue)
 
         os.makedirs(os.path.dirname(filename), exist_ok=True)
         with open(filename, 'w') as f:
             cfg.write(f)
@@ -214,26 +232,62 @@
         for pat in options:
             for sect, opts in self._parse_opt(pat):
                 self._remove(sect, opts, local, name)
 
     def run(self, options=None, local=True, name=None):
         lines = []
 
-        if options:
-            for pat in options:
-                for sect, opts in self._parse_opt(pat):
+        if options and len(options) == 1 and options[0].find('=') == -1:
+            for sect, opts in self._parse_opt(options[0]):
+                title = 'Section: %s' % sect
+                lines.extend(['', '-' * 60, title])
+                self.infos = [], [], [], []
+
+                for opt in opts:
+                    self._list_value(sect, opt, local, name)
+
+                lines.extend(['', 'Current settings'])
+                lines.extend(self.infos[0])
+                lines.extend(['', 'Global settings'])
+                lines.extend(self.infos[1])
+                lines.extend(['', 'Local settings'])
+                lines.extend(self.infos[2])
+                if name:
+                    lines.extend(['', 'Private "%s" settings' % name])
+                    lines.extend(self.infos[3])
+
+        elif options:
+            pairs = []
+            prev, op = None, ''
+            for opt in options:
+                i = opt.find('=')
+                if i > 0:
+                    pairs.append([opt[:i], opt[i+1:]])
+                elif opt in ('+', '=', '-', '^'):
+                    op = opt
+                elif prev:
+                    pairs.append((prev, op + opt))
+                    prev, op = None, ''
+                else:
+                    prev = opt
+            if prev:
+                raise CliError('no value for option "%s"' % prev)
+
+            for pat, value in pairs:
+                sect_opts = self._parse_opt(pat)
+                if not sect_opts:
+                    logger.debug('new builder option "%s"', pat)
+                    sect_opts = [('builder', [pat])]
+                for sect, opts in sect_opts:
                     title = 'Section: %s' % sect
                     lines.extend(['', '-' * 60, title])
                     self.infos = [], [], [], []
 
                     for opt in opts:
-                        if opt.find('=') == -1:
-                            self._list_value(sect, opt, local, name)
-                        else:
-                            self._set_option(sect, opt, local, name)
+                        self._set_option(sect, opt, value, local, name)
 
                     lines.extend(['', 'Current settings'])
                     lines.extend(self.infos[0])
                     lines.extend(['', 'Global settings'])
                     lines.extend(self.infos[1])
                     lines.extend(['', 'Local settings'])
                     lines.extend(self.infos[2])
```

## pyarmor/cli/context.py

```diff
@@ -34,15 +34,15 @@
 
 runtime_package_template2 = '''# Pyarmor $rev, $timestamp
 for suffix in '', '_a1', '_a2', '_a3':
     try:
         __pyarmor__ = __import__('pyarmor_runtime' + suffix,
                                  globals(), locals(),
                                  ('__pyarmor__',),
-                                 0)
+                                 0).__pyarmor__
         break
     except ModuleNotFoundError:
         pass
 else:
     raise ModuleNotFoundError('no pyarmor_runtime extension found')
 '''
 
@@ -126,18 +126,20 @@
         self.module_builtins = set()
 
         self.obfuscated_modules = set()
         self.extra_libs = {}
 
         self.rft_auto_excludes = set(['super'])
         self.rft_export_names = set()
+        self.rft_transform_op = '?'
 
         self.runtime_key = None
 
         self.cmd_options = {}
+        self.plugins = []
 
     def _read_config(self, filelist, encoding=None):
         cfg = configparser.ConfigParser(
             empty_lines_in_values=False,
             interpolation=configparser.ExtendedInterpolation(),
         )
         cfg.read(filelist, encoding=encoding)
@@ -158,14 +160,18 @@
             f.write(data)
 
     def clear_token(self):
         if os.path.exists(self.license_token):
             with open(self.license_token, 'wb') as f:
                 f.close()
 
+    def group_device_file(self, devid):
+        filename = 'pyarmor-group-device.%s' % devid
+        return os.path.join(self.local_path, 'group', filename)
+
     def read_license(self):
         if os.path.exists(self.license_file):
             with open(self.license_file, 'rb') as f:
                 return f.read()
 
     def push(self, options):
         finder = {}
@@ -220,15 +226,15 @@
         verinfo = ['%s (%s)' % (rev, lictype)]
 
         if verbose > 1:
             verinfo.append(licinfo['licno'][-6:])
 
         if verbose > 2:
             pname = licinfo['product']
-            verinfo.append('non-profits' if pname in ('', 'TBD') else pname)
+            verinfo.append(pname)
 
         if verbose > 3:
             regname = licinfo['regname']
             if regname:
                 verinfo.append(regname)
 
         return ', '.join(verinfo)
@@ -312,17 +318,14 @@
             self.cfg['logging'].get('debug_logfile', 'pyarmor.debug.log'))
 
     @property
     def trace_logfile(self):
         return self._check_logpath(
             self.cfg['logging'].get('trace_logfile', 'pyarmor.trace.log'))
 
-    def trace_rftfile(self, name):
-        return self._check_logpath(os.path.join(self.local_path, 'rft', name))
-
     def _optb(self, section, name):
         return self.cfg.getboolean(section, name, vars=self.cmd_options)
 
     def _opts(self, section, name):
         return self.cfg.get(section, name, vars=self.cmd_options)
 
     def _opti(self, section, name):
@@ -500,26 +503,79 @@
         return self._opti('runtime', 'timer')
 
     @property
     def runtime_simple_extension_name(self):
         return self._optb('runtime', 'simple_extension_name')
 
     @property
-    def runtime_hooks(self):
-        value = self._rt_opt('hooks')
-        if value:
-            from ast import literal_eval
-            name, encoding = (value + ':utf-8').split(':')[:2]
-            for x in self.local_path, self.global_path:
-                filename = os.path.join(x, name)
-                if os.path.exists(filename):
-                    with open(filename, encoding=encoding) as f:
-                        return literal_eval(f.read())
+    def runtime_user_data(self):
+        data = b''
+        filename = self.cmd_options.get('user_data')
+        if filename:
+            if filename[0] == '@':
+                with open(filename[1:], 'rb') as f:
+                    data = f.read()
+            else:
+                data = filename.encode()
+
+        hook = b''
+        filename = os.path.join(self.local_path, 'hooks', 'pyarmor_runtime.py')
+        if os.path.exists(filename):
+            with open(filename, 'rb') as f:
+                hook = f.read()
+
+        return hook, data
 
     @property
     def runtime_messages(self):
         value = self.cfg['runtime'].get('messages', '')
         if value:
             name, encoding = (value + ':utf-8').split(':')[:2]
             cfg = self._named_config(name, encoding=encoding)
             if cfg.has_section('runtime.message'):
                 return cfg
+
+    #
+    # RFT settings
+    #
+
+    def rft_output_script(self, name):
+        return self._check_logpath(os.path.join(self.local_path, 'rft', name))
+
+    def rft_set_exclude_table(self, encoding=None):
+        filename = os.path.join(self.local_path, 'rft_exclude_table')
+        os.makedirs(os.path.dirname(filename), exist_ok=True)
+        with open(filename, 'w', encoding=encoding) as f:
+            f.write(' '.join(self.rft_auto_excludes))
+
+    def rft_get_exclude_table(self, encoding=None):
+        filename = os.path.join(self.local_path, 'rft_exclude_table')
+        if os.path.exists(filename):
+            with open(filename, encoding=encoding) as f:
+                return f.read().split()
+        return []
+
+    #
+    # BCC settings
+    #
+
+    @property
+    def bcc_build_path(self):
+        path = os.path.join(self.local_path, 'bcc')
+        os.makedirs(path, exist_ok=True)
+        return path
+
+    #
+    # Plugin and hook
+    #
+    def runtime_hook(self, modname):
+        for path in self.local_path, self.global_path:
+            filename = os.path.join(path, 'hooks', modname + '.py')
+            if os.path.exists(filename):
+                encoding = self.cfg['builder'].get('encoding', 'utf-8')
+                with open(filename, encoding=encoding) as f:
+                    return f.read()
+
+    def runtime_plugin(self, source, target, platforms):
+        for plugin in self.plugins:
+            if hasattr(plugin, 'post_runtime'):
+                plugin.post_runtime(self, source, target, platforms)
```

## pyarmor/cli/default.cfg

```diff
@@ -1,17 +1,17 @@
 [pyarmor]
 
 ;; Pyarmor version
 major = 8
-minor = 1
+minor = 2
 patch = 0
 
 ;; Core version
-core = 2.1
-runtime = 2.1
+cli.core = 3.2
+cli.runtime = 3.2
 
 ;; Default timeout when send request to remote server for
 ;;     check Pyarmor license
 ;;     register Pyarmor license
 timeout = 6
 
 regurl = https://api.dashingsoft.com/product/key/enter/%s/?
@@ -35,20 +35,14 @@
 data_files = 0
 
 ;;
 ;; How to find dependent packages
 ;;
 findall = 0
 
-;; Extra paths to find dependent package
-; pypaths =
-
-;; List module names couldn't be found automically
-; hidden_imports =
-
 [builder]
 ;;
 ;; Part 1: only global/local settings, not in module level
 ;;
 
 ;; File encoding to read scripts
 encoding = utf-8
@@ -83,19 +77,38 @@
 ;; How many loops for jit iv
 jit_iv_threshold = 100
 
 ;; Now "argument" is not available
 rft_enables = builtin import function class method global local
 
 ;; Exclude unknown attrs automically
+;    0     disable auto exclude, use auto include
+;    1     auto exclude and load .pyarmor/rft/exclude_table
+;    2     auto exclude but not load exclude_table
 rft_auto_exclude = 1
 
+;; Export all the names in module attribute __all__
+rft_auto_export = 1
+
+;; Enable dev mode for rft
+rft_dev_mode = 0
+
 ;; Export module and classes
 ; rft_export_names = pkg.mod pkg.mod.cls pkg.mod.attr
 
+;; Extra paths to find dependent package
+; pypaths =
+
+;; List module names couldn't be found automically
+; hidden_imports =
+
+;; If it's enabled, disable some features to make scripts work with nuitka
+;; convenient settings for nuitka, but now it's TBD
+; support_nuitka = 0
+
 ;;
 ;; Part 2: global/local/module level options
 ;;
 
 ;; The argument optimize specifies the optimization level of the
 ;; compiler; the default value of -1 selects the optimization level of
 ;; the interpreter as given by -O options. Explicit levels are 0 (no
@@ -118,14 +131,15 @@
 assert_import = 0
 
 ;; mix string constant
 mix_str = 0
 
 mix_coname = 0
 mix_localnames = 1
+;; Enable it may result in annotations error
 mix_argnames = 0
 
 obf_module = 1
 obf_code = 1
 wrap_mode = 1
 
 restrict_module = 1
@@ -157,15 +171,15 @@
 
 ;; Whether encrypt name in statement import
 rft_mix_import_name = 0
 
 [runtime]
 
 ;; Generate extension for all Python3.7+
-universal = false
+universal = 0
 
 ;; The file ext only keep .so/.pyd, for example
 ;;     pyarmor_runtime.cpython-37m-darwin.so
 ;;     if simple_extension_name == 1 then
 ;;     pyarmor_runtime.so
 simple_extension_name = 1
 
@@ -223,30 +237,32 @@
 ;; Target platforms
 ; platforms =
 
 ;; If there are customized runtime messages
 messages = messages.cfg:utf-8
 
 [assert.call]
-enables = all
+;; and: function is in obfuscated script and match ruler
+;;  or: function is in obfuscated script or match ruler
+auto_mode = and
 
 ; includes =
 ; excludes =
 
 [assert.import]
-enables = all
+;; and: module is obfuscated and match ruler
+;;  or: module is obfuscated or match ruler
+auto_mode = and
 
 ; includes =
 ; excludes =
 
 [mix.str]
-enables = all
-
 ;; do not mix short string len(s) < this value
-threshold = 4
+threshold = 8
 
 ; includes =
 ; excludes =
 
 [pack]
 ;; Strip output path to match archive info
 strip = 0
@@ -261,34 +277,16 @@
 ;; How to do when the obfuscated module has no matched .pyc in bundle
 ;;    error, issue a error and exit
 ;;    warning, issue a warning and continue
 ;;    ignore, do nothing
 ;;    append, append it to archive
 no_matched_pyc = error
 
-[windows.x86_64.bcc]
-cc = clang.exe
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-windows -c
-
-[linux.x86_64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
-
-[linux.aarch64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib
-linker_script = ${bcc:linker_script}
-
-[darwin.x86_64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-gnu_linux -fPIC -c
-
-[darwin.aarch64.bcc]
-cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=arm64-macho-darwin -fPIC -fno-addrsig -fno-stack-protector -shared -nostdlib -lsystem -T${bcc:tempdir}/darwin.aarch64.ldscript
-linker_script = ${bcc:linker_script}
-
 [bcc]
-unsupported_functions = exec eval super locals
+unsupported_functions = exec eval super locals __assert_armored__
 unsupported_nodes = AsyncFunctionDef AsyncFor AsyncWith Await Yield YieldFrom GeneratorExp NamedExpr MatchValue MatchSingleton MatchSequence MatchMapping MatchClass MatchStar MatchAs MatchOr
 
 ;; Exclude co_names
 ; excludes =
 
 ;; Use opcode CALL_FUNCTION_EX to patch call
 ;; Global option, all scripts must be same
@@ -305,29 +303,22 @@
 
 ;; Use op_mkfunc2 to build unsupported functions
 enable_pure_function = 1
 
 ;; Convert comprehensions to bcc code
 enable_comprehension = 1
 
-tempdir = .pyarmor/bcc
-linker_script = /* pyarmor bcc mode link script */
-    SECTIONS {
-       . = 0x1000;
-       PROVIDE (_scode = .);
-       .text           : { *(.text) }
-       .data           : { *(.data) }
-       .rodata         : { *(.rodata) }
-       .got            : { *(.got) }
-       .got.plt        : { *(.got.plt) }
-       .imptbl         : { *(.imptbl) }
-       .explt          : { *(.explt) }
-       PROVIDE (_ecode = .);
-       .note.gnu.build-id      : { *(.note.gnu.build-id) }
-       .note.gnu.property      : { *(.note.gnu.property) }
-       .gnu.hash               : { *(.gnu.hash) }
-       .dynsym                 : { *(.dynsym) }
-       .dynstr                 : { *(.dynstr) }
-       .rela.dyn               : { *(.rela.dyn) }
-       .dynamic                : { *(.dynamic) }
-       .comment                : { *(.comment) }
-    }
+[windows.x86_64.bcc]
+cc = clang.exe
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-windows -c
+
+[linux.x86_64.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -c
+
+[linux.aarch64.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables -fPIC -fno-stack-protector -shared -nostdlib -Tlinux.aarch64.ldscript
+
+[darwin.x86_64.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=x86_64-elf-gnu_linux -fPIC -c
+
+[darwin.aarch64.bcc]
+cflags = -O3 -Wno-unsequenced -fno-asynchronous-unwind-tables -fno-unwind-tables --target=arm64-macho-darwin -fPIC -fno-addrsig -fno-stack-protector -shared -nostdlib -lsystem
```

## pyarmor/cli/generate.py

```diff
@@ -15,24 +15,21 @@
 #
 #  @File: cli/generate.py
 #
 #  @Author: Jondy Zhao (pyarmor@163.com)
 #
 #  @Create Date: 2022-12-06
 #
-import logging
 import os
 import shutil
 
-from .errors import CliError
+from . import logger, CliError
 from .core import Pytransform3
 from .resource import FileResource, PathResource
 
-logger = logging.getLogger('Builder')
-
 
 class Finder(object):
 
     def __init__(self, ctx):
         self.ctx = ctx
 
     def prepare(self, input_paths):
@@ -85,20 +82,20 @@
     def generate_runtime_package(self, output):
         if self.ctx.runtime_key is None:
             self.ctx.runtime_key = self.generate_runtime_key()
         Pytransform3.generate_runtime_package(self.ctx, output)
 
     def _pack_script(self, bundle, output, entry=None, codesign=None):
         from .repack import repacker
-        build = os.path.join('.pyarmor', 'build')
-        repacker(bundle, output, build, entry=entry, codesign=codesign)
-        shutil.rmtree(build)
+        buildpath = os.path.join('.pyarmor', 'pack')
+        repacker(bundle, output, buildpath, entry=entry, codesign=codesign)
+        shutil.rmtree(buildpath)
 
     def _obfuscate_scripts(self):
-        rev = self.ctx.version_info(verbose=2)
+        rev = self.ctx.version_info()
         template = self.ctx.bootstrap_template
         relative = self.ctx.import_prefix
         pkgname = self.ctx.runtime_package + self.ctx.runtime_suffix
         bootpath = self.ctx.cfg.get('builder', 'bootstrap_file')
 
         namelist = []
         for res in self.ctx.resources:
```

## pyarmor/cli/mixer.py

```diff
@@ -16,20 +16,17 @@
 #  @File: cli/mixer.py
 #
 #  @Author: Jondy Zhao (pyarmor@163.com)
 #
 #  @Create Date: 2022-12-06
 #
 import ast
-import logging
 
 from random import randint
 
-logger = logging.getLogger('Mixer')
-
 
 class StrNodeTransformer(ast.NodeTransformer):
 
     def _reform_str(self, s):
         encoding = getattr(self, 'encoding')
         value = bytearray(s.encode(encoding) if encoding else s.encode())
         key = [randint(0, 255)] * len(value)
```

## pyarmor/cli/register.py

```diff
@@ -15,36 +15,34 @@
 #
 #  @File: cli/register.py
 #
 #  @Author: Jondy Zhao (pyarmor@163.com)
 #
 #  @Create Date: Mon Jan  2 15:39:08 CST 2023
 #
-import logging
 import os
 
 from base64 import b64decode, urlsafe_b64encode
 from json import loads as json_loads
 from string import Template
 
-
-logger = logging.getLogger('Pyarmor')
+from . import logger, CliError
 
 
 def parse_token(data):
     from struct import unpack
 
     if not data or data.find(b' ') == -1:
         return {
             'token': 0,
             'rev': 0,
             'features': 0,
             'licno': 'pyarmor-vax-000000',
             'regname': '',
-            'product': '',
+            'product': 'non-profits',
             'note': 'This is trial license'
         }
 
     buf = b64decode(data.split()[0])
 
     token, value = unpack('II', buf[:8])
     rev, features = value & 0xff, value >> 8
@@ -54,49 +52,50 @@
     i = 64
     for k in range(4):
         n = buf[i]
         i += 1
         pstr.append(buf[i:i+n].decode('utf-8') if n else '')
         i += n
 
+    product = 'non-profits(TBD)' if pstr[2] in ('', 'TBD') else pstr[2]
     return {
         'token': token,
         'rev': rev,
         'features': features,
         'licno': licno,
         'machine': pstr[0],
         'regname': pstr[1],
-        'product': pstr[2],
+        'product': product,
         'note': pstr[3],
     }
 
 
 class Register(object):
 
     def __init__(self, ctx):
         self.ctx = ctx
         self.notes = []
 
     def check_args(self, args):
         if args.upgrade and args.keyfile.endswith('.zip'):
-            raise RuntimeError('use .txt file to upgrade, not .zip file')
+            raise CliError('use .txt file to upgrade, not .zip file')
 
     def _get_old_rcode(self):
         old_license = self.ctx.read_license()
         if not old_license:
             logger.debug('no license file found')
             return
         if len(old_license) == 256:
             logger.debug('no old purchased license')
             return
 
         data = b64decode(old_license)
         i = data.find(b'pyarmor-vax-')
         if i == -1:
-            raise RuntimeError('no valid old license')
+            raise CliError('no valid old license')
         return data[i:i+18].decode()
 
     def regurl(self, ucode, product=None, rcode=None, prepare=False):
         url = self.ctx.cfg['pyarmor']['regurl'] % ucode
         if product:
             url += '&product=' + \
                 urlsafe_b64encode(product.encode('utf-8')).decode()
@@ -115,21 +114,22 @@
     @property
     def license_info(self):
         return parse_token(self.ctx.read_token())
 
     def _license_type(self, info):
         return 'basic' if info['features'] == 1 else \
             'pro' if info['features'] == 7 else \
+            'group' if info['features'] == 15 else \
             'trial' if info['token'] == 0 else 'unknown'
 
     def _license_to(self, info):
         name = info['regname']
         product = info['product']
         return '%s (%s)' % (product, name) if name and product else \
-            '' if not name else 'non-profits (%s)' % name
+            'non-profits' if not name else 'non-profits (%s)' % name
 
     def parse_keyfile(self, filename):
         with open(filename, 'r', encoding='utf-8') as f:
             for line in f:
                 line = line.strip()
                 marker = 'Dear '
                 if line.startswith(marker):
@@ -137,84 +137,122 @@
                     break
 
             for line in f:
                 line = line.strip()
                 if len(line) == 192 and line.find(' ') == -1:
                     return regname, line
 
-        raise RuntimeError('no registration code found in %s' % filename)
+        raise CliError('no registration code found in %s' % filename)
 
     def register_regfile(self, regfile, clean=True):
         from zipfile import ZipFile
 
-        path = self.ctx.home_path
+        path = self.ctx.reg_path
         with ZipFile(regfile, 'r') as f:
             for item in ('license.lic', '.pyarmor_capsule.zip'):
-                logger.debug('extracting %s' % item)
+                logger.debug('extracting %s', item)
                 f.extract(item, path=path)
+            namelist = f.namelist()
+            if 'group.tokens' in namelist:
+                machid = self._get_machine_id()
+                name = '/'.join(['tokens', machid.decode('utf-8')])
+                if name not in namelist:
+                    logger.debug('no found "%s" in offline regfile', name)
+                    raise CliError('this regfile is not for this device')
+                logger.debug('extracting %s', name)
+                self.ctx.save_token(f.read(name))
+                return
+            if 'group.info' in namelist:
+                raise CliError('wrong usage for group license, please '
+                               'check `pyarmor reg` in Man page')
 
         logger.info('update license token')
         self.update_token()
 
+    def _get_machine_id(self):
+        from .core import Pytransform3
+        return Pytransform3.get_hd_info(10)
+
+    def generate_group_device(self, devid):
+        path = self.ctx.group_device_file(devid)
+        logger.info('generating device file "%s"', path)
+        os.makedirs(os.path.dirname(path), exist_ok=True)
+        with open(path, "wb") as f:
+            f.write(b'machine: ' + self._get_machine_id())
+        return path
+
     def __str__(self):
         '''$advanced
 
 Notes
-* Internet connection is required to verify Pyarmor license
 $notes
 '''
 
         info = self.license_info
         lictype = self._license_type(info)
 
         fmt = '%-16s: %s'
         lines = [
             fmt % ('License Type', 'pyarmor-' + lictype),
             fmt % ('License No.', info['licno']),
-            fmt % ('License To', self._license_to(info)),
+            fmt % ('License To', info['regname']),
+            fmt % ('License Product', info['product']),
             '',
         ]
 
         bccmode = info['features'] & 2
         rftmode = info['features'] & 4
         advanced = [
             fmt % ('BCC Mode', 'Yes' if bccmode else 'No'),
             fmt % ('RFT Mode', 'Yes' if rftmode else 'No'),
         ]
         if lictype == 'trial':
-            self.notes.append(
-                '* Trial license can\'t obfuscate big script and mix str'
-            )
+            self.notes.append('* Can\'t obfuscate big script and mix str')
+        elif lictype in ('bacic', 'pro'):
+            self.notes.append('* Each obfuscation need verify license online')
+        elif lictype == 'group':
+            self.notes.append('* Offline obfuscation')
 
         lines.append(Template(self.__str__.__doc__).substitute(
             advanced='\n'.join(advanced),
             notes='\n'.join(self.notes),
         ))
 
         return '\n'.join(lines)
 
 
 upgrade_to_basic_info = Template('''
-You are about to upgrade old Pyarmor license to Pyarmor Basic
-License for Pyarmor 8.0+
+You are about to upgrade old Pyarmor license to Pyarmor Basic License
 
 The upgraded license information will be''')
 
 upgrade_to_pro_info = Template('''
-You are about to upgrade old Pyarmor license to Pyarmor Pro
-License for Pyarmor 8.0+
+You are about to upgrade old Pyarmor license to Pyarmor Pro License
 
 The original license no: $rcode
 
 The upgraded license information will be''')
 
 
 class WebRegister(Register):
 
+    def _request(self, url):
+        from http.client import HTTPSConnection
+        n = len('https://')
+        k = url.find('/', n)
+        conn = HTTPSConnection(url[n:k])
+        conn.request("GET", url[k:])
+        return conn.getresponse()
+
     def _send_request(self, url, timeout=6.0):
+        try:
+            return self._request(url)
+        except Exception as e:
+            logger.debug('direct request failed "%s"', str(e))
+
         from urllib.request import urlopen
         from ssl import _create_unverified_context
         context = _create_unverified_context()
         return urlopen(url, None, timeout, context=context)
 
     def _remove_token(self):
         if os.path.exists(self.ctx.license_token):
@@ -222,55 +260,75 @@
             os.remove(self.ctx.license_token)
 
     def prepare(self, keyfile, product, upgrade=False):
         reginfo = self.parse_keyfile(keyfile)
         logger.info('prepare "%s"', keyfile)
 
         rcode = self._get_old_rcode() if upgrade else None
+        if upgrade and keyfile.endswith('regcode-to-pro.txt'):
+            logger.error('please use `pyarmor-7 -v` to check old license')
+            logger.error('this code is used to upgrade old license')
+            raise CliError('no found old license in this machine')
         url = self.regurl(reginfo[1], rcode=rcode, prepare=True)
         logger.debug('url: %s', url)
 
         logger.info('query key file from server')
-        res = self._send_request(url)
-        if not res:
-            raise RuntimeError('no response from license server')
-        if res.code != 200:
-            raise RuntimeError(res.read().decode('utf-8'))
-
-        info = json_loads(res.read())
-        if info['product'] not in ('', 'TBD') and \
-           product and product != info['product']:
-            raise RuntimeError(
-                'product name has been set to "%s"' % info['product'])
-        if info['product'] in ('', 'TBD'):
-            info['product'] = product if product else 'TBD'
+        with self._send_request(url) as res:
+            if not res:
+                logger.error('please try it later')
+                raise CliError('no response from license server')
+            if res.code != 200:
+                logger.error('HTTP Error %s', res.code)
+                raise CliError(res.read().decode('utf-8'))
+            info = json_loads(res.read())
+
+        pname = info['product']
+        if pname in ('', 'TBD'):
+            info['product'] = product
+        elif pname != product:
+            logger.warning('this license is bind to product "%s"', pname)
+            logger.warning('it can not be changed to "%s"', product)
 
         lines = []
         if upgrade:
             if not (rcode and rcode.startswith('pyarmor-vax-')):
-                raise RuntimeError('old code "%s" can not be upgraded' % rcode)
+                logger.error('please check Pyarmor 8.0 EULA')
+                raise CliError('old code "%s" can not be upgraded' % rcode)
             if info['upgrade']:
                 lines.append(upgrade_to_pro_info.substitute(rcode=rcode))
             else:
                 lines.append(upgrade_to_basic_info.substitute())
         else:
             if info['lictype'] not in ('BASIC', 'PRO', 'GROUP'):
-                raise RuntimeError('unknown license type %s' % info['lictype'])
+                logger.error('this license does not work in Pyarmor 8')
+                logger.error('please check Pyarmor 8.0 EULA')
+                raise CliError('unknown license type %s' % info['lictype'])
             lines.append('This license registration information will be')
 
+        if info['product'] in ('', 'TBD') and info['lictype'] == 'GROUP':
+            raise CliError('"TBD" is invalid product name for group license')
+
         fmt = '%-16s: %s'
         lines.extend([
             '',
             fmt % ('License Type', 'pyarmor-' + info['lictype'].lower()),
-            fmt % ('License Owner', info['regname']),
-            fmt % ('Bind Product', info['product']),
+            fmt % ('License To', info['regname']),
+            fmt % ('License Product', info['product']),
             '',
         ])
-        if info['product'] in ('', 'TBD'):
+        if info['product'] == 'non-profits':
             lines.append('This license is about to be used for non-profits')
+        elif info['product'] in ('', 'TBD'):
+            lines.append('This license is bind to non-profits(TBD) '
+                         'for the time being')
+            lines.append('If not change "TBD" to product name in 6 months, '
+                         'it will be set to "non-profits" automatically')
+        else:
+            lines.append('This license is about to be used for product "%s"'
+                         % info['product'])
 
         lines.extend(['', ''])
         return info, '\n'.join(lines)
 
     def upgrade_to_pro(self, keyfile, product):
         logger.info('process upgrading file "%s"', keyfile)
         reginfo = self.parse_keyfile(keyfile)
@@ -285,22 +343,19 @@
         res = self._send_request(url)
         regfile = self._handle_response(res)
 
         logger.info('update license token')
         self.update_token()
         logger.info('This license has been upgraded successfully')
 
-        notes = (
-            '* Please backup regfile "%s" carefully, and '
-            'use this file for next registration' % regfile,
-            '* Please do not upgrade this code again'
-        )
-        logger.info('Import Notes:\n\n%s', '\n'.join(notes))
+        notes = '* Please backup regfile "%s" carefully, and ' \
+            'use this file for subsequent registration' % regfile,
+        logger.info('Import Notes:\n\n%s\n', notes)
 
-    def register(self, keyfile, product, upgrade=False):
+    def register(self, keyfile, product, upgrade=False, group=False):
         if keyfile.endswith('.zip'):
             logger.info('register "%s"', keyfile)
             self.register_regfile(keyfile)
             return
 
         logger.info('process activation file "%s"', keyfile)
         reginfo = self.parse_keyfile(keyfile)
@@ -310,33 +365,113 @@
             url += '&upgrade_to_basic=1'
         logger.debug('url: %s', url)
 
         logger.info('send request to server')
         res = self._send_request(url)
         regfile = self._handle_response(res)
 
-        logger.info('register "%s"', regfile)
-        self.register_regfile(regfile)
+        notes = [
+            '* Please backup regfile "%s" carefully, and '
+            'use this file for subsequent registration' % regfile,
+            '* Do not use "%s" again' % os.path.basename(keyfile),
+        ]
 
-        logger.info('This license has been %s successfully',
-                    'upgraded' if upgrade else 'registered')
+        if group:
+            logger.info('This group license has been activated sucessfully')
+            notes.append('* Please check `pyarmor reg` in Man page for '
+                         'how to register Pyarmor on offline device')
+        else:
+            logger.info('register "%s"', regfile)
+            self.register_regfile(regfile)
+            logger.info('This license code has been %s successfully',
+                        'upgraded' if upgrade else 'activated')
 
-        notes = (
-            '* Please backup regfile "%s" carefully, and '
-            'use this file for next registration' % regfile,
-            '* "%s" can be used only 10 times' % os.path.basename(keyfile),
-        )
-        logger.info('Import Notes:\n\n%s', '\n'.join(notes))
+        logger.info('Import Notes:\n\n%s\n', '\n'.join(notes))
 
     def _handle_response(self, res):
         if res and res.code == 200:
             dis = res.headers.get('Content-Disposition')
             filename = dis.split('"')[1] if dis else 'pyarmor-regfile.zip'
             logger.info('write registration file "%s"', filename)
-            with open(filename, 'wb') as f:
-                f.write(res.read())
+            data = res.read()
+            if data.startswith(b'{"group":'):
+                n = data.find(b'}') + 1
+                with open(filename, 'wb') as f:
+                    f.write(data[n:])
+                self._write_group_info(filename, data[:n])
+            else:
+                with open(filename, 'wb') as f:
+                    f.write(data)
             return filename
 
         elif res:
-            raise RuntimeError(res.read().decode('utf-8'))
+            raise CliError(res.read().decode('utf-8'))
+
+        raise CliError('no response from license server')
+
+    def _write_group_info(self, filename, data):
+        from zipfile import ZipFile
+        logger.info('write group information')
+        with ZipFile(filename, 'a') as f:
+            f.writestr('group.info', data)
+
+    def register_group_device(self, regfile, devid, rev=1):
+        from zipfile import ZipFile
+        devfile = self.ctx.group_device_file(devid)
+        logger.info('register device file "%s"', devfile)
+        logger.info('use group license "%s"', regfile)
+        if not os.path.exists(devfile):
+            logger.error('please generate device file in offline device by')
+            logger.error('    pyarmor reg -g %s', devid)
+            logger.error('and copy generated device file to this machine')
+            raise CliError('no group device file "%s"' % devfile)
+
+        with open(devfile) as f:
+            prefix = 'machine:'
+            for line in f:
+                if line.startswith(prefix):
+                    machid = line[len(prefix):].strip()
+                    break
+            else:
+                logger.error('no machid information in device file')
+                raise CliError('invalid device file "%s"' % devfile)
+
+        with ZipFile(regfile, 'r') as f:
+            if 'group.info' not in f.namelist():
+                logger.error('no group information in group license file')
+                raise CliError('invalid group license file "%s"' % regfile)
+            group = json_loads(f.read('group.info'))
+            licdata = f.read('license.lic')
+            capsule = f.read('.pyarmor_capsule.zip')
+
+        tokencache = os.path.join(os.path.dirname(devfile), 'tokens', machid)
+        if os.path.exists(tokencache):
+            logger.info('read cached "%s"', tokencache)
+            with open(tokencache, 'rb') as f:
+                data = f.read()
+            filename = regfile.replace('pyarmor-', 'pyarmor-device-').replace(
+                '.zip', '.%s.zip' % devid)
+            logger.info('write registeration file "%s"', filename)
+        else:
+            logger.info('send request to server')
+            url = self.regurl('/'.join(['group', group['ucode']]))
+            paras = ('rev', str(rev)), ('group', str(group['group'])), \
+                ('source', machid), ('devid', str(devid))
+            url += '&'.join(['='.join(x) for x in paras])
+            logger.debug('url: %s', url)
+
+            res = self._send_request(url)
+            filename = self._handle_response(res)
+            with open(filename, 'rb') as f:
+                data = f.read()
+            os.makedirs(os.path.dirname(tokencache), exist_ok=True)
+            with open(tokencache, 'wb') as f:
+                f.write(data)
+
+        with ZipFile(filename, 'w') as f:
+            f.writestr('license.lic', licdata)
+            f.writestr('.pyarmor_capsule.zip', capsule)
+            f.writestr('group.tokens', b'')
+            f.writestr('tokens/' + machid, data)
 
-        raise RuntimeError('no response from license server')
+        logger.info('please copy deivce regfile to offline device and run')
+        logger.info('    pyarmor reg %s', filename)
```

## pyarmor/cli/repack.py

```diff
@@ -15,15 +15,15 @@
     from PyInstaller.loader.pyimod02_archive import PYZ_TYPE_PKG
 except ModuleNotFoundError:
     from PyInstaller.loader.pyimod01_archive import ZlibArchiveReader
     from PyInstaller.loader.pyimod01_archive import PYZ_TYPE_PKG
 from PyInstaller.compat import is_darwin, is_linux, is_win
 
 
-logger = logging.getLogger('Packer')
+logger = logging.getLogger('repack')
 
 
 class ZlibArchive(ZlibArchiveReader):
 
     def checkmagic(self):
         """ Overridable.
             Check to see if the file object self.lib actually has a file
```

## pyarmor/cli/resource.py

```diff
@@ -171,30 +171,31 @@
         recursive = options.get('recursive', False)
         includes = options.get('includes', '').split()
         excludes = options.get('excludes', '').split()
         patterns = options.get('data_files', '').split()
 
         def in_filter(path, name):
             fullpath = os.path.join(path, name)
+            ext = os.path.splitext(name)[1]
             return not ex_filter(path, name) and (
-                os.path.splitext(name)[1] in pyexts
+                (ext and ext in pyexts)
                 or any([fnmatch(fullpath, x) for x in includes]))
 
         def ex_filter(path, name):
             fullpath = os.path.join(path, name)
             return excludes and any([fnmatch(fullpath, x) for x in excludes])
 
         def is_res(path, name):
             s = os.path.join(path, name)
             return any([fnmatch(s, x) for x in patterns])
 
         for path, dirnames, filenames in os.walk(self.fullpath):
             self.resfiles = [x for x in [
-                Resource(name, parent=self) if is_res(path, name)
-                else FileResource(name, parent=self) if in_filter(path, name)
+                FileResource(name, parent=self) if in_filter(path, name)
+                else Resource(name, parent=self) if is_res(path, name)
                 else None for name in filenames
             ] if x]
             self.respaths = [PathResource(name, parent=self)
                              for name in dirnames
                              if not ex_filter(path, name)]
             break
```

## Comparing `pyarmor.cli-8.1.dev9.dist-info/METADATA` & `pyarmor.cli-8.2.dev1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli
-Version: 8.1.dev9
+Version: 8.2.dev1
 Summary: A comand line tool to obfuscate python scripts
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Keywords: protect obfuscate encrypt obfuscation distribute
 Platform: UNKNOWN
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Software Distribution
-Requires-Dist: pyarmor.core (~=1.0)
+Requires-Dist: pyarmor.core (~=2.1.0)
 
 Protect Python Scripts By Pyarmor
 =================================
 
 Pyarmor is a command line tool used to obfuscate python scripts, bind
 obfuscated scripts to fixed machine or expire obfuscated scripts.
```

## Comparing `pyarmor.cli-8.1.dev9.dist-info/RECORD` & `pyarmor.cli-8.2.dev1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-pyarmor/cli/__init__.py,sha256=ewQIh0wc49TeewnGYkGsG_ALFMA_g314F4Ad7fRlktM,1292
-pyarmor/cli/__main__.py,sha256=uyTndUm2mpiTcjCP5XO4SeCqD2LskS00MtOF_OBguBg,20090
-pyarmor/cli/config.py,sha256=HbCIOkJ2Zd7aGeanB1tUpBhWTj1LhyMiSwWGdmFgN0A,8608
-pyarmor/cli/context.py,sha256=Onjz-5zEsdumN0GkpEJGH0ld24W5m6SjqZRpGRnm-KE,15562
-pyarmor/cli/default.cfg,sha256=i-EM_E4Ee1rU6yBq8a00eZEKI8moRow9ZFKr_i6Gd7s,7736
-pyarmor/cli/errors.py,sha256=gNlPhcqgCS4OVdU9H8V23YxThyvHKtFI3LKAu-sxH60,880
-pyarmor/cli/generate.py,sha256=7GnIcVG2G8MlaH60-7a2UcCsyedu5Cr0OH_IoOix_GQ,5603
-pyarmor/cli/mixer.py,sha256=CQOttISF-h55lWEbRUaywsNZybxe8KsXC7axO1ISxUE,4008
+pyarmor/cli/__init__.py,sha256=YcZi3LC9kB4LevpDabYvJWszFYoILXSrt6JQWW0EivI,1479
+pyarmor/cli/__main__.py,sha256=K1YRvlGGv5C_mzq5q26R0HASFIVkG1JgGUrTkyTpD8Q,22591
+pyarmor/cli/config.py,sha256=wOiXqsnnowYUhMMPzWPZZN8aJPa-K7JJJHDxdz9cbt8,10694
+pyarmor/cli/context.py,sha256=WL1e4UETx95a3imjrQQUaQULpkdIeIqbbSTTLYv0aQg,17255
+pyarmor/cli/default.cfg,sha256=aVux3Nsp5JOjMGyUJG4XrI_0XCkgS91cCiNtljWBnTQ,7475
+pyarmor/cli/generate.py,sha256=4IQU0JQ7f7Gr6SCpqnT9VEB4-jex8hHq-sf_5ULEVfQ,5553
+pyarmor/cli/mixer.py,sha256=i4IrXukoG5L3V3Wv5BgDSTkNU5NB03-Q4bgsWwug6LY,3956
+pyarmor/cli/plugin.py,sha256=1bgFhdn5pVHCVfvRTiwstK9B817PcKPC1q_NvXtGnlg,2847
 pyarmor/cli/public_capsule.zip,sha256=1r4u42ixfocGPMQc0OklpoHF3nvVW6GA1f4SwcEJWVI,2487
-pyarmor/cli/register.py,sha256=fNtET8fjd1KxypZ34E9sy9zIA3wkmy2kI57bkDe7saA,10980
-pyarmor/cli/repack.py,sha256=JTmb-KAzPLNu_VttJTym53uJg5GJlPkmNZQ-LjM8gS8,11386
-pyarmor/cli/resource.py,sha256=ef-2nvRhlyYOlSub6LbYywnmABFmtCAADRcK6j89Udg,6366
+pyarmor/cli/register.py,sha256=YpjurGEkQYhLmAQS-plvRWG_HqS4wFGqQMu9uBD0n6U,17413
+pyarmor/cli/repack.py,sha256=cbTFqNJYo2NZE1hDInKoj3FtZpCwWCeADQNGto-tn1o,11386
+pyarmor/cli/resource.py,sha256=yzHLAKvtF3rlg747CDBLkohbc5_cmp4uWGxRHWYfJXA,6398
 pyarmor/cli/shell.py,sha256=S1yJ5RQZhTIysQgXk3H4E_cJsV2Lymh-w-_GdnHFngU,2193
-pyarmor.cli-8.1.dev9.dist-info/METADATA,sha256=tglg14h4D3Cn-LG0HvYdQfGCHz7dXaiw2Dvf4ZtHFMQ,2405
-pyarmor.cli-8.1.dev9.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
-pyarmor.cli-8.1.dev9.dist-info/entry_points.txt,sha256=MODwyeC-iHX4KItYshzQRa5kWWQnMhIuT64w5bqKFR0,41
-pyarmor.cli-8.1.dev9.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli-8.1.dev9.dist-info/RECORD,,
+pyarmor.cli-8.2.dev1.dist-info/METADATA,sha256=MI6Jl0cQHuHWfisz0aT5LADvOXjAWvvKrWPkSziY56I,2407
+pyarmor.cli-8.2.dev1.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
+pyarmor.cli-8.2.dev1.dist-info/entry_points.txt,sha256=MODwyeC-iHX4KItYshzQRa5kWWQnMhIuT64w5bqKFR0,41
+pyarmor.cli-8.2.dev1.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli-8.2.dev1.dist-info/RECORD,,
```


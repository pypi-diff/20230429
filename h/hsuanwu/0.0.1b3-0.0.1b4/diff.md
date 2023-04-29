# Comparing `tmp/hsuanwu-0.0.1b3.tar.gz` & `tmp/hsuanwu-0.0.1b4.tar.gz`

## Comparing `hsuanwu-0.0.1b3.tar` & `hsuanwu-0.0.1b4.tar`

### file list

```diff
@@ -1,540 +1,227 @@
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/ACKNOWLEDGMENT.md
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/CONTRIBUTING.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/Makefile
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/mkdocs.yml
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.github/FUNDING.yml
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.github/ISSUE_TEMPLATE/documentation.yml
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.github/ISSUE_TEMPLATE/question.yml
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.github/workflows/ci.yml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/.gitignore
--rw-r--r--   0        0        0    16434 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/.ninja_log
--rw-r--r--   0        0        0    48415 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/build.ninja
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/default.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.__init__.imports
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.__init__.imports
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.engine.__init__.imports
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.engine.__init__.imports-1
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.engine.base_policy_trainer.imports
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.engine.distributed_trainer.imports
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.engine.distributed_trainer.imports-1
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.engine.off_policy_trainer.imports
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.engine.off_policy_trainer.imports-1
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.engine.on_policy_trainer.imports
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.engine.on_policy_trainer.imports-1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.engine.utils.imports
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.logger.imports
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.common.timer.imports
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.env.__init__.imports
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.env.atari.__init__.imports
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.env.atari.wrappers.imports
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.env.bullet.__init__.imports
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.env.dmc.__init__.imports
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.env.dmc.natural_imgsource.imports
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.env.dmc.wrappers.imports
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.env.minigrid.__init__.imports
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.env.procgen.__init__.imports
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.env.utils.imports
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.evaluation.__init__.imports
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.evaluation.comparison.imports
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.evaluation.performance.imports
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.evaluation.utils.imports
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.evaluation.visualization.imports
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.__init__.imports
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.agent.__init__.imports
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.agent.base.imports
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.agent.drqv2.imports
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.agent.impala.imports
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.agent.network.imports
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.agent.ppg.imports
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.agent.ppo.imports
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.agent.sac.imports
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.agent.utils.imports
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.encoder.__init__.imports
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.encoder.base.imports
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.encoder.espeholt_residual_encoder.imports
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.encoder.identity_encoder.imports
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.encoder.mnih_cnn_encoder.imports
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.encoder.tassa_cnn_encoder.imports
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.encoder.vanilla_mlp_encoder.imports
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.storage.__init__.imports
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.storage.base.imports
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.storage.distributed_storage.imports
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.storage.nstep_replay_storage.imports
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.storage.prioritized_replay_storage.imports
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.storage.utils.imports
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.storage.vanilla_replay_storage.imports
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xploit.storage.vanilla_rollout_storage.imports
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.__init__.imports
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.__init__.imports
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.auto_augment.imports
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.base.imports
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.elastic_transform.imports
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.gaussian_noise.imports
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.grayscale.imports
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_adjustsharpness.imports
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_amplitude_scaling.imports
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_augment.imports
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_autocontrast.imports
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_colorjitter.imports
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_convolution.imports
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_crop.imports
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_cutout.imports
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_cutoutcolor.imports
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_equalize.imports
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_flip.imports
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_invert.imports
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_perspective.imports
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_rotate.imports
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_shift.imports
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.augmentation.random_translate.imports
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.__init__.imports
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.__init__.imports-1
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.base.imports
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.categorical.imports
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.categorical.imports-1
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.diagonal_gaussian.imports
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.kl.imports
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.kl.imports-1
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.normal_noise.imports
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.ornstein_uhlenbeck_noise.imports
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.squashed_normal.imports
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.truncated_normal_noise.imports
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.distribution.utils.imports
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.__init__.imports
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.__init__.imports-1
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.base.imports
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.girm.imports
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.icm.imports
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.ngu.imports
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.pseudo_counts.imports
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.pseudo_counts.imports-1
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.re3.imports
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.revd.imports
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.ride.imports
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.rise.imports
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/hsuanwu.xplore.reward.rnd.imports
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/imports/npu_ppo.imports
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/npu_ppo.pyi
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/__init__.pyi
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/__init__.pyi
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/logger.pyi
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/timer.pyi
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/engine/__init__.pyi
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/engine/__init__.pyi-1
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/engine/base_policy_trainer.pyi
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/engine/distributed_trainer.pyi
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/engine/distributed_trainer.pyi-1
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/engine/off_policy_trainer.pyi
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/engine/off_policy_trainer.pyi-1
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/engine/on_policy_trainer.pyi
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/engine/on_policy_trainer.pyi-1
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/common/engine/utils.pyi
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/env/__init__.pyi
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/env/utils.pyi
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/env/atari/__init__.pyi
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/env/atari/wrappers.pyi
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/env/bullet/__init__.pyi
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/env/dmc/__init__.pyi
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/env/dmc/natural_imgsource.pyi
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/env/dmc/wrappers.pyi
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/env/minigrid/__init__.pyi
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/env/procgen/__init__.pyi
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/evaluation/__init__.pyi
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/evaluation/comparison.pyi
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/evaluation/performance.pyi
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/evaluation/utils.pyi
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/evaluation/visualization.pyi
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/__init__.pyi
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/agent/__init__.pyi
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/agent/base.pyi
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/agent/drqv2.pyi
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/agent/impala.pyi
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/agent/network.pyi
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/agent/ppg.pyi
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/agent/ppo.pyi
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/agent/sac.pyi
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/agent/utils.pyi
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/encoder/__init__.pyi
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/encoder/base.pyi
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/encoder/espeholt_residual_encoder.pyi
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/encoder/identity_encoder.pyi
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/encoder/mnih_cnn_encoder.pyi
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/encoder/tassa_cnn_encoder.pyi
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/encoder/vanilla_mlp_encoder.pyi
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/storage/__init__.pyi
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/storage/base.pyi
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/storage/distributed_storage.pyi
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/storage/nstep_replay_storage.pyi
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/storage/prioritized_replay_storage.pyi
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/storage/utils.pyi
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/storage/vanilla_replay_storage.pyi
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xploit/storage/vanilla_rollout_storage.pyi
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/__init__.pyi
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/__init__.pyi
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/auto_augment.pyi
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/base.pyi
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/elastic_transform.pyi
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/gaussian_noise.pyi
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/grayscale.pyi
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_adjustsharpness.pyi
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_amplitude_scaling.pyi
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_augment.pyi
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_autocontrast.pyi
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_colorjitter.pyi
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_convolution.pyi
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_crop.pyi
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_cutout.pyi
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_cutoutcolor.pyi
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_equalize.pyi
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_flip.pyi
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_invert.pyi
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_perspective.pyi
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_rotate.pyi
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_shift.pyi
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/augmentation/random_translate.pyi
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/__init__.pyi
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/__init__.pyi-1
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/base.pyi
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/categorical.pyi
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/categorical.pyi-1
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/diagonal_gaussian.pyi
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/kl.pyi
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/kl.pyi-1
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/normal_noise.pyi
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.pyi
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/squashed_normal.pyi
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/truncated_normal_noise.pyi
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/distribution/utils.pyi
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/__init__.pyi
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/__init__.pyi-1
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/base.pyi
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/girm.pyi
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/icm.pyi
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/ngu.pyi
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/pseudo_counts.pyi
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/pseudo_counts.pyi-1
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/re3.pyi
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/revd.pyi
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/ride.pyi
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/rise.pyi
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.pytype/pyi/hsuanwu/xplore/reward/rnd.pyi
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/1371cdf75b5e614f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/1378ebcbf13907f7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/13fb16aa84b797dd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/19b01ebee9a847fc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/1a5e8029e4a9e31f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/1ac3f1dff5514509
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/1ba9be091bd5fdcf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/1fcd777a364d27f3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/2022ed3b9b57977e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/25703fb8e0d412ed
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/26e9a832810a16e8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/29634a2848d96ea7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/2a834dddb817788d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/2d9eced4ab87f900
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/2e983c5ee8042cc8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/2fd7f0cb172ac8e1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/30c2450e5751b63
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/32efa579a32f31e7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/339482a12766fda1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/3a62418feb13ee68
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/4061bd2219abae48
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/40c1dbddc37b04fe
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/44b43d2630fd9430
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/455eabc1b82a768d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/4635f338fc608ac7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/4fac13595b4ef343
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/59723800dc929b59
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/60ed929db2a14bc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/665a2d3d8aa15d65
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/6b6948608aedd884
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/6bde106b7147e32f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/6c6680e4d50924bd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/715c645c3462405c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/72db8d8e3e62ae69
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/75f7ae405e877754
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/7628cab189ec6e54
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/771f44c75a7bfd7c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/780d90c692cfb559
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/7a3cb5faa7c3c0ed
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/7c34098018047b23
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/7cec1a19862cd424
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/7d5b5fa180e8d244
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/7edae10b312f55d5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/80fc0e1707464180
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/83125fbbf4fe5b2b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/84c1d6dfcb730d5e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/85ba6a9cf5e04908
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/88c01598af9ca03d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/8a2719f00eaae50c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/8e16ac2e9a4df350
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/8e252cd5ca328296
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/8e42af03a9cea277
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/8e902be760538c4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/8f2fe811d3e35c80
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/8f34527aecdd109
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/9144a7867bb3d059
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/94cd4cda5ef8a21
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/9aa421df035ca4a8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/a22e8cdfc573573e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/a493c57472c0b89
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/a7e529d7b1771bcf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/a8a6e9a44a28f421
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/a8f4c35627b0669d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/aab32152d4b6b5d5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/ac1f46e25ff511e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/ae81fae1451238d5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/b06b3cc496e16026
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/b1c2b8941182a3ea
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/b25238cfe0927613
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/b430e350baddacd1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/b487473f3137324a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/b9aff20203f58f09
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/bba4ec6251c724ba
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/bd6893e6bbb66601
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/c0d467f210fb4818
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/c32ec96e7c7075ce
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/c332fd93c7e25f29
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/c5abb47155d91c99
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/c85305cbf817b695
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/ca2344d18c07346b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/cdf980c872c4e39f
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/cf4904885992eebf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/d32fe21965ece9b9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/d525cc7d3eac6a2b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/d7f7db139957a176
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/e3d9f2cf95f8701c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/e6f6edeb83a8a908
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/ed35c69f8f764087
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/eddaafa2c668b722
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/ef13d9a1da22be81
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/ef87298fe9f7004e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/effd88f186b1a4db
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/f184f23734b27cc8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/f22867f62d21038d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/f61882ca936af230
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/f732c3bf7137fcaa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/f8f12f04e9099924
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/f9edefbc5e4306ad
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/fa57c7f5fd6646c4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/fb1c1c25f01a5a9a
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/fe74590a6ed3f366
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.ruff_cache/content/ff566c617ef7ca27
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/deployment/__init__.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/CNAME
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/benchmarks.md
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/changelog.md
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/contributing.md
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/generate_mkgendocs.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/getting_started.md
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/index.md
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/license.md
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/mkgendocs.yml
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/trigger.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/tutorials.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/verification.md
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/contributing.md
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/index.md
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/common/logger.md
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/common/timer.md
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/common/engine/__init__.md
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/common/engine/base_policy_trainer.md
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/common/engine/distributed_trainer.md
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/common/engine/off_policy_trainer.md
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/common/engine/on_policy_trainer.md
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/env/utils.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/env/atari/__init__.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/env/bullet/__init__.md
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/env/dmc/__init__.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/env/minigrid/__init__.md
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/env/procgen/__init__.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/evaluation/comparison.md
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/evaluation/performance.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/agent/base.md
--rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/agent/drqv2.md
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/agent/impala.md
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/agent/ppg.md
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/agent/ppo.md
--rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/agent/sac.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/encoder/base.md
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/encoder/espeholt_residual_encoder.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/encoder/identity_encoder.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/encoder/mnih_cnn_encoder.md
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/encoder/tassa_cnn_encoder.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/encoder/vanilla_mlp_encoder.md
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/storage/distributed_storage.md
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/storage/nstep_replay_storage.md
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/storage/prioritized_replay_storage.md
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/storage/vanilla_replay_storage.md
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xploit/storage/vanilla_rollout_storage.md
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/auto_augment.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/base.md
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/elastic_transform.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/gaussian_noise.md
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/grayscale.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_adjustsharpness.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_amplitude_scaling.md
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_augment.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_autocontrast.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_colorjitter.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_convolution.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_crop.md
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_cutout.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_cutoutcolor.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_equalize.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_flip.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_invert.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_perspective.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_rotate.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_shift.md
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_translate.md
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/distribution/base.md
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/distribution/categorical.md
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/distribution/diagonal_gaussian.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/distribution/kl.md
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/distribution/normal_noise.md
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/distribution/ornstein_uhlenbeck_noise.md
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/distribution/squashed_normal.md
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/distribution/truncated_normal_noise.md
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/reward/base.md
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/reward/girm.md
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/reward/icm.md
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/reward/ngu.md
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/reward/pseudo_counts.md
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/reward/re3.md
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/reward/revd.md
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/reward/ride.md
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/reward/rise.md
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/api/xplore/reward/rnd.md
--rw-r--r--   0        0        0    81827 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/assets/images/github_issues.png
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/assets/images/icon.svg
--rw-r--r--   0        0        0    94410 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/assets/images/logo.png
--rw-r--r--   0        0        0   152927 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/assets/images/qq.jpg
--rw-r--r--   0        0        0    70288 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/assets/images/rl_training.png
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/assets/images/roadmap.svg
--rw-r--r--   0        0        0    81227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/assets/images/slack.png
--rw-r--r--   0        0        0    17517 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/assets/images/structure.svg
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/assets/stylesheets/extra.css
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/overview/api.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/overview/common_index/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/overview/deployment_index/index.md
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/overview/env_index/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/overview/evaluation_index/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/overview/pretraining_index/index.md
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/overview/xploit_index/index.md
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/docs/overview/xplore_index/index.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/common/__init__.py
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/common/logger.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/common/timer.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/common/engine/__init__.py
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/common/engine/base_policy_trainer.py
--rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/common/engine/distributed_trainer.py
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/common/engine/off_policy_trainer.py
--rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/common/engine/on_policy_trainer.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/common/engine/utils.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/env/__init__.py
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/env/utils.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/env/atari/__init__.py
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/env/atari/wrappers.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/env/bullet/__init__.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/env/dmc/__init__.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/env/dmc/natural_imgsource.py
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/env/dmc/wrappers.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/env/minigrid/__init__.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/env/procgen/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/evaluation/__init__.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/evaluation/comparison.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/evaluation/performance.py
--rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/evaluation/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/evaluation/visualization.py
--rw-r--r--   0        0        0    16422 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/experimental/npu_ppo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/__init__.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/agent/__init__.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/agent/base.py
--rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/agent/drqv2.py
--rw-r--r--   0        0        0    12307 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/agent/impala.py
--rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/agent/network.py
--rw-r--r--   0        0        0    15125 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/agent/ppg.py
--rw-r--r--   0        0        0    10240 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/agent/ppo.py
--rw-r--r--   0        0        0    13609 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/agent/sac.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/agent/utils.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/__init__.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/base.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/espeholt_residual_encoder.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/identity_encoder.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/mnih_cnn_encoder.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/tassa_cnn_encoder.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/vanilla_mlp_encoder.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/storage/__init__.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/storage/base.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/storage/distributed_storage.py
--rw-r--r--   0        0        0     8793 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/storage/nstep_replay_storage.py
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/storage/prioritized_replay_storage.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/storage/utils.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/storage/vanilla_replay_storage.py
--rw-r--r--   0        0        0     7960 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xploit/storage/vanilla_rollout_storage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/__init__.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/auto_augment.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/base.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/elastic_transform.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/gaussian_noise.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/grayscale.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_adjustsharpness.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_amplitude_scaling.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_augment.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_autocontrast.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_colorjitter.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_convolution.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_crop.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_cutout.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_cutoutcolor.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_equalize.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_flip.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_invert.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_perspective.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_rotate.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_shift.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_translate.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/__init__.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/base.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/categorical.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/diagonal_gaussian.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/kl.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/normal_noise.py
--rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/squashed_normal.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/truncated_normal_noise.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/utils.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/__init__.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/base.py
--rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/girm.py
--rw-r--r--   0        0        0     9843 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/icm.py
--rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/ngu.py
--rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/pseudo_counts.py
--rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/re3.py
--rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/revd.py
--rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/ride.py
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/rise.py
--rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/hsuanwu/xplore/reward/rnd.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/scripts/run_tests.sh
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/tests/test_aug.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/tests/test_dist.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/tests/test_env.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/tests/test_eval.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/tests/test_logger.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/tests/test_mp.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/tests/test_reward.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/tests/test_torch.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/.gitignore
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/LICENSE
--rw-r--r--   0        0        0    12423 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/README.md
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/pyproject.toml
--rw-r--r--   0        0        0    14244 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b3/PKG-INFO
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/ACKNOWLEDGMENT.md
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/Makefile
+-rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/mkdocs.yml
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/documentation.yml
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/question.yml
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/deployment/__init__.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/CNAME
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/benchmarks.md
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/changelog.md
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/contributing.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/generate_mkgendocs.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/getting_started.md
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/index.md
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/license.md
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/mkgendocs.yml
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/trigger.yml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/verification.md
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/contributing.md
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/index.md
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/logger.md
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/timer.md
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/engine/__init__.md
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/engine/base_policy_trainer.md
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/engine/distributed_trainer.md
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/engine/off_policy_trainer.md
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/common/engine/on_policy_trainer.md
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/utils.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/atari/__init__.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/bullet/__init__.md
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/dmc/__init__.md
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/minigrid/__init__.md
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/env/procgen/__init__.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/evaluation/comparison.md
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/evaluation/performance.md
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/base.md
+-rw-r--r--   0        0        0     3752 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/drqv2.md
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/impala.md
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/ppg.md
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/ppo.md
+-rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/agent/sac.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/base.md
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/espeholt_residual_encoder.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/identity_encoder.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/mnih_cnn_encoder.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/tassa_cnn_encoder.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/encoder/vanilla_mlp_encoder.md
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/storage/distributed_storage.md
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/storage/nstep_replay_storage.md
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/storage/prioritized_replay_storage.md
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/storage/vanilla_replay_storage.md
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xploit/storage/vanilla_rollout_storage.md
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/auto_augment.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/base.md
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/elastic_transform.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/gaussian_noise.md
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/grayscale.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_adjustsharpness.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_amplitude_scaling.md
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_augment.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_autocontrast.md
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_colorjitter.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_convolution.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_crop.md
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_cutout.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_cutoutcolor.md
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_equalize.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_flip.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_invert.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_perspective.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_rotate.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_shift.md
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_translate.md
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/base.md
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/categorical.md
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/diagonal_gaussian.md
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/kl.md
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/normal_noise.md
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/ornstein_uhlenbeck_noise.md
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/squashed_normal.md
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/distribution/truncated_normal_noise.md
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/base.md
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/girm.md
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/icm.md
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/ngu.md
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/pseudo_counts.md
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/re3.md
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/revd.md
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/ride.md
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/rise.md
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/api/xplore/reward/rnd.md
+-rw-r--r--   0        0        0    81827 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/github_issues.png
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/icon.svg
+-rw-r--r--   0        0        0    94410 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/logo.png
+-rw-r--r--   0        0        0   152927 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/qq.jpg
+-rw-r--r--   0        0        0    70288 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/rl_training.png
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/roadmap.svg
+-rw-r--r--   0        0        0    81227 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/slack.png
+-rw-r--r--   0        0        0    17517 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/images/structure.svg
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/assets/stylesheets/extra.css
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/api.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/common_index/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/deployment_index/index.md
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/env_index/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/evaluation_index/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/pretraining_index/index.md
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/xploit_index/index.md
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/overview/xplore_index/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/tutorials/configuration.md
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/tutorials/index.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/docs/tutorials/quick_start.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/__init__.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/verification.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/__init__.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/logger.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/timer.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/__init__.py
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/base_policy_trainer.py
+-rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/distributed_trainer.py
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/off_policy_trainer.py
+-rw-r--r--   0        0        0     7019 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/on_policy_trainer.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/common/engine/utils.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/__init__.py
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/utils.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/atari/__init__.py
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/atari/wrappers.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/bullet/__init__.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/dmc/__init__.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/dmc/natural_imgsource.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/dmc/wrappers.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/minigrid/__init__.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/env/procgen/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/evaluation/__init__.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/evaluation/comparison.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/evaluation/performance.py
+-rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/evaluation/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/evaluation/visualization.py
+-rw-r--r--   0        0        0    16422 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/experimental/npu_ppo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/__init__.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/__init__.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/base.py
+-rw-r--r--   0        0        0     9558 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/drqv2.py
+-rw-r--r--   0        0        0    12307 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/impala.py
+-rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/network.py
+-rw-r--r--   0        0        0    15125 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/ppg.py
+-rw-r--r--   0        0        0    10240 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/ppo.py
+-rw-r--r--   0        0        0    13609 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/sac.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/agent/utils.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/__init__.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/base.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/espeholt_residual_encoder.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/identity_encoder.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/mnih_cnn_encoder.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/tassa_cnn_encoder.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/vanilla_mlp_encoder.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/__init__.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/base.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/distributed_storage.py
+-rw-r--r--   0        0        0     8793 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/nstep_replay_storage.py
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/prioritized_replay_storage.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/utils.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/vanilla_replay_storage.py
+-rw-r--r--   0        0        0     7960 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xploit/storage/vanilla_rollout_storage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/__init__.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/auto_augment.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/base.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/elastic_transform.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/gaussian_noise.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/grayscale.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_adjustsharpness.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_amplitude_scaling.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_augment.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_autocontrast.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_colorjitter.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_convolution.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_crop.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_cutout.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_cutoutcolor.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_equalize.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_flip.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_invert.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_perspective.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_rotate.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_shift.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_translate.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/__init__.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/base.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/categorical.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/diagonal_gaussian.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/kl.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/normal_noise.py
+-rw-r--r--   0        0        0     4066 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/squashed_normal.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/truncated_normal_noise.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/utils.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/__init__.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/base.py
+-rw-r--r--   0        0        0    13152 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/girm.py
+-rw-r--r--   0        0        0     9843 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/icm.py
+-rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/ngu.py
+-rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/pseudo_counts.py
+-rw-r--r--   0        0        0     5866 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/re3.py
+-rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/revd.py
+-rw-r--r--   0        0        0    11748 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/ride.py
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/rise.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/hsuanwu/xplore/reward/rnd.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/scripts/run_tests.sh
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_aug.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_dist.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_env.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_eval.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_logger.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_mp.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_reward.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/tests/test_torch.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/.gitignore
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/LICENSE
+-rw-r--r--   0        0        0    12440 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/README.md
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/pyproject.toml
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 hsuanwu-0.0.1b4/PKG-INFO
```

### Comparing `hsuanwu-0.0.1b3/ACKNOWLEDGMENT.md` & `hsuanwu-0.0.1b4/ACKNOWLEDGMENT.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/CODE_OF_CONDUCT.md` & `hsuanwu-0.0.1b4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/CONTRIBUTING.md` & `hsuanwu-0.0.1b4/docs/api/contributing.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/Makefile` & `hsuanwu-0.0.1b4/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,14 @@
 	isort --check ${LINT_PATHS}
 	# Reformat using black
 	black --check ${LINT_PATHS}
 
 commit-checks: format type lint
 
 build:
-	python3 -m build
+	python -m build
 
 twine:
-	python3 -m twine upload --repository pypi dist/*
+	python -m twine upload --repository pypi dist/*
 
 gendocs:
 	gendocs --config docs/mkgendocs.yml
```

### Comparing `hsuanwu-0.0.1b3/mkdocs.yml` & `hsuanwu-0.0.1b4/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -64,49 +64,51 @@
     - Contribution: contributing.md
     - License: license.md
 
   - Getting Started:
     - Installation: getting_started.md
     - Verification: verification.md
   
-  - Tutorials: tutorials.md
+  - Tutorials: 
+    - Overview: tutorials/index.md
 
   - API Documentation:
     - Overview: overview/api.md
     - Common: 
+      - Common Overview: overview/common_index/index.md
       - Engine: 
         - HsuanwuEngine: api/common/engine/__init__.md
-        - BasePolicyTrainer: api/common/base_policy_trainer.md
-        - OnPolicyTrainer: api/common/on_policy_trainer.md
-        - OffPolicyTrainer: api/common/off_policy_trainer.md
-        - DistributedTrainer: api/common/distributed_trainer.md
+        - BasePolicyTrainer: api/common/engine/base_policy_trainer.md
+        - OnPolicyTrainer: api/common/engine/on_policy_trainer.md
+        - OffPolicyTrainer: api/common/engine/off_policy_trainer.md
+        - DistributedTrainer: api/common/engine/distributed_trainer.md
       - Logger: api/common/logger.md
       - Timer: api/common/timer.md
 
     - Xploit:
       - Xploit Overview: overview/xploit_index/index.md
-      - encoder:
-        - BaseEncoder: api/xploit/encoder/base.md
-        - TassaCnnEncoder: api/xploit/encoder/tassa_cnn_encoder.md
-        - MnihCnnEncoder: api/xploit/encoder/mnih_cnn_encoder.md
-        - EspeholtResidualEncoder: api/xploit/encoder/espeholt_residual_encoder.md
-        - VanillaMlpEncoder: api/xploit/encoder/vanilla_mlp_encoder.md
-        - IdentityEncoder: api/xploit/encoder/identity_encoder.md
-
       - agent:
         - BaseAgent: api/xploit/agent/base.md
         - SAC: api/xploit/agent/sac.md
         - DrQ: api/xploit/agent/sac.md
         - DrQv2: api/xploit/agent/drqv2.md
         - DDPG: api/xploit/agent/drqv2.md
         - PPG: api/xploit/agent/ppg.md
         - PPO: api/xploit/agent/ppo.md
         - DrAC: api/xploit/agent/ppo.md
         - IMPALA: api/xploit/agent/impala.md
       
+      - encoder:
+        - BaseEncoder: api/xploit/encoder/base.md
+        - TassaCnnEncoder: api/xploit/encoder/tassa_cnn_encoder.md
+        - MnihCnnEncoder: api/xploit/encoder/mnih_cnn_encoder.md
+        - EspeholtResidualEncoder: api/xploit/encoder/espeholt_residual_encoder.md
+        - VanillaMlpEncoder: api/xploit/encoder/vanilla_mlp_encoder.md
+        - IdentityEncoder: api/xploit/encoder/identity_encoder.md
+
       - storage:
         - DistributedStorage: api/xploit/storage/distributed_storage.md
         - VanillaRolloutStorage: api/xploit/storage/vanilla_rollout_storage.md
         - VanillaReplayStorage: api/xploit/storage/vanilla_replay_storage.md
         - NStepReplayStorage: api/xploit/storage/nstep_replay_storage.md
         - PrioritizedReplayStorage: api/xploit/storage/prioritized_replay_storage.md
 
@@ -147,30 +149,30 @@
         - RandomTranslate: api/xplore/augmentation/random_translate.md
 
       - distribution:
         - BaseDistribution: api/xplore/distribution/base.md
         - Categorical: api/xplore/distribution/categorical.md
         - DiagonalGaussian: api/xplore/distribution/diagonal_gaussian.md
         - SquashedNormal: api/xplore/distribution/squashed_normal.md
-        - NormalNoise: api/xplore/distribution/truncated_normal_noise.md
+        - NormalNoise: api/xplore/distribution/normal_noise.md
         - OrnsteinUhlenbeckNoise: api/xplore/distribution/ornstein_uhlenbeck_noise.md
         - TruncatedNormalNoise: api/xplore/distribution/truncated_normal_noise.md
     
     - Env:
-      - Overview: overview/env_index/index.md
-      - make_atari_env: api/env/atari.md
+      - Env Overview: overview/env_index/index.md
+      - make_atari_env: api/env/atari/__init__.md
       - make_bullet_env: api/env/bullet/__init__.md
       - make_dmc_env: api/env/dmc/__init__.md
       - make_procgen_env: api/env/procgen/__init__.md
       - make_minigrid_env: api/env/minigrid/__init__.md
       - utils:
         - HsuanwuEnvWrapper: api/env/utils.md
     
     - Evaluation:
-      - Overview: overview/evaluation_index/index.md
+      - Evaluation Overview: overview/evaluation_index/index.md
       - Comparison: api/evaluation/comparison.md
       - Performance: api/evaluation/performance.md
 
     - Pre-training: 
       - Pre-training Overview: overview/pretraining_index/index.md
     
     - Deployment:
```

### Comparing `hsuanwu-0.0.1b3/.github/FUNDING.yml` & `hsuanwu-0.0.1b4/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/.github/PULL_REQUEST_TEMPLATE.md` & `hsuanwu-0.0.1b4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/.github/ISSUE_TEMPLATE/bug_report.yml` & `hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/.github/ISSUE_TEMPLATE/documentation.yml` & `hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/documentation.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/.github/ISSUE_TEMPLATE/feature_request.yml` & `hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/.github/ISSUE_TEMPLATE/question.yml` & `hsuanwu-0.0.1b4/.github/ISSUE_TEMPLATE/question.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/.github/workflows/ci.yml` & `hsuanwu-0.0.1b4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/contributing.md` & `hsuanwu-0.0.1b4/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 To run tests with `pytest`:
 
 ```
 make pytest
 ```
 
-Type checking with `pytype` and `mypy`:
+Type checking with `pytype`:
 
 ```
 make type
 ```
 
 Codestyle check with `black`, `isort` and `ruff`:
```

### Comparing `hsuanwu-0.0.1b3/docs/generate_mkgendocs.py` & `hsuanwu-0.0.1b4/docs/generate_mkgendocs.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/index.md` & `hsuanwu-0.0.1b4/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -145,32 +145,57 @@
 00000900: 7374 7261 7465 7320 7468 6520 6d61 696e  strates the main
 00000910: 2065 766f 6c75 7469 6f6e 2072 6f61 646d   evolution roadm
 00000920: 6170 206f 6620 4873 7561 6e77 753a 0d0a  ap of Hsuanwu:..
 00000930: 3c64 6976 2061 6c69 676e 3d63 656e 7465  <div align=cente
 00000940: 723e 0d0a 3c69 6d67 2073 7263 3d27 2e2f  r>..<img src='./
 00000950: 6173 7365 7473 2f69 6d61 6765 732f 726f  assets/images/ro
 00000960: 6164 6d61 702e 7376 6727 3e0d 0a3c 2f64  admap.svg'>..</d
-00000970: 6976 3e0d 0a0d 0a3c 212d 2d20 506c 6561  iv>....<!-- Plea
-00000980: 7365 2063 6974 6520 7468 6520 666f 6c6c  se cite the foll
-00000990: 6f77 696e 6720 7061 7065 7220 6966 2079  owing paper if y
-000009a0: 6f75 2075 7365 2048 7375 616e 7775 2069  ou use Hsuanwu i
-000009b0: 6e20 796f 7572 2077 6f72 6b2c 2074 6861  n your work, tha
-000009c0: 6e6b 2079 6f75 210d 0a60 6060 6269 6274  nk you!..```bibt
-000009d0: 6578 0d0a 4061 7274 6963 6c65 7b79 7561  ex..@article{yua
-000009e0: 6e32 3032 3368 7375 616e 7775 2c0d 0a20  n2023hsuanwu,.. 
-000009f0: 2074 6974 6c65 3d7b 4873 7561 6e77 753a   title={Hsuanwu:
-00000a00: 204c 6f6e 672d 5465 726d 2045 766f 6c75   Long-Term Evolu
-00000a10: 7469 6f6e 2050 726f 6a65 6374 206f 6620  tion Project of 
-00000a20: 5265 696e 666f 7263 656d 656e 7420 4c65  Reinforcement Le
-00000a30: 6172 6e69 6e67 7d2c 0d0a 2020 6175 7468  arning},..  auth
-00000a40: 6f72 3d7b 5975 616e 2c20 4d69 6e67 7169  or={Yuan, Mingqi
-00000a50: 2061 6e64 204c 756f 2c20 5368 6968 616f   and Luo, Shihao
-00000a60: 2061 6e64 205a 6861 6e67 2c20 5a65 7175   and Zhang, Zequ
-00000a70: 6e20 616e 6420 5961 6e67 2c20 5875 2061  n and Yang, Xu a
-00000a80: 6e64 204a 696e 2c20 5869 6e20 616e 6420  nd Jin, Xin and 
-00000a90: 4c69 2c20 426f 2061 6e64 205a 656e 672c  Li, Bo and Zeng,
-00000aa0: 2057 656e 6a75 6e7d 2c0d 0a20 206a 6f75   Wenjun},..  jou
-00000ab0: 726e 616c 3d7b 6172 5869 7620 7072 6570  rnal={arXiv prep
-00000ac0: 7269 6e74 2061 7258 6976 3a32 3331 312e  rint arXiv:2311.
-00000ad0: 3135 3237 377d 2c0d 0a20 2079 6561 723d  15277},..  year=
-00000ae0: 7b32 3032 337d 0d0a 7d0d 0a60 6060 202d  {2023}..}..``` -
-00000af0: 2d3e                                     ->
+00000970: 6976 3e0d 0a0d 0a4a 6f69 6e20 7468 6520  iv>....Join the 
+00000980: 6465 7665 6c6f 7065 7220 636f 6d6d 756e  developer commun
+00000990: 6974 7920 666f 7220 6973 7375 6573 2061  ity for issues a
+000009a0: 6e64 2064 6973 6375 7373 696f 6e73 3a0d  nd discussions:.
+000009b0: 0a0d 0a7c 536c 6163 6b7c 5151 7c47 6974  ...|Slack|QQ|Git
+000009c0: 4875 627c 0d0a 7c3a 2d3a 7c3a 2d3a 7c3a  Hub|..|:-:|:-:|:
+000009d0: 2d3a 7c0d 0a7c 3c61 2068 7265 663d 2268  -:|..|<a href="h
+000009e0: 7474 7073 3a2f 2f61 7070 2e73 6c61 636b  ttps://app.slack
+000009f0: 2e63 6f6d 2f63 6c69 656e 742f 5430 3534  .com/client/T054
+00000a00: 4a34 4e4a 5850 302f 4330 3534 5437 3851  J4NJXP0/C054T78Q
+00000a10: 5a39 4122 3e3c 696d 6720 7372 633d 272e  Z9A"><img src='.
+00000a20: 2f61 7373 6574 732f 696d 6167 6573 2f73  /assets/images/s
+00000a30: 6c61 636b 2e70 6e67 2720 7374 796c 653d  lack.png' style=
+00000a40: 2277 6964 7468 3a20 3530 2522 203e 3c2f  "width: 50%" ></
+00000a50: 613e 7c3c 696d 6720 7372 633d 272e 2f61  a>|<img src='./a
+00000a60: 7373 6574 732f 696d 6167 6573 2f71 712e  ssets/images/qq.
+00000a70: 6a70 6727 2073 7479 6c65 3d22 7769 6474  jpg' style="widt
+00000a80: 683a 2036 3525 223e 7c3c 6120 6872 6566  h: 65%">|<a href
+00000a90: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+00000aa0: 2e63 6f6d 2f52 4c45 2d46 6f75 6e64 6174  .com/RLE-Foundat
+00000ab0: 696f 6e2f 4873 7561 6e77 752f 6973 7375  ion/Hsuanwu/issu
+00000ac0: 6573 223e 3c69 6d67 2073 7263 3d27 2e2f  es"><img src='./
+00000ad0: 6173 7365 7473 2f69 6d61 6765 732f 6769  assets/images/gi
+00000ae0: 7468 7562 5f69 7373 7565 732e 706e 6727  thub_issues.png'
+00000af0: 2073 7479 6c65 3d22 7769 6474 683a 2035   style="width: 5
+00000b00: 3025 223e 3c2f 613e 7c0d 0a0d 0a3c 212d  0%"></a>|....<!-
+00000b10: 2d20 506c 6561 7365 2063 6974 6520 7468  - Please cite th
+00000b20: 6520 666f 6c6c 6f77 696e 6720 7061 7065  e following pape
+00000b30: 7220 6966 2079 6f75 2075 7365 2048 7375  r if you use Hsu
+00000b40: 616e 7775 2069 6e20 796f 7572 2077 6f72  anwu in your wor
+00000b50: 6b2c 2074 6861 6e6b 2079 6f75 210d 0a60  k, thank you!..`
+00000b60: 6060 6269 6274 6578 0d0a 4061 7274 6963  ``bibtex..@artic
+00000b70: 6c65 7b79 7561 6e32 3032 3368 7375 616e  le{yuan2023hsuan
+00000b80: 7775 2c0d 0a20 2074 6974 6c65 3d7b 4873  wu,..  title={Hs
+00000b90: 7561 6e77 753a 204c 6f6e 672d 5465 726d  uanwu: Long-Term
+00000ba0: 2045 766f 6c75 7469 6f6e 2050 726f 6a65   Evolution Proje
+00000bb0: 6374 206f 6620 5265 696e 666f 7263 656d  ct of Reinforcem
+00000bc0: 656e 7420 4c65 6172 6e69 6e67 7d2c 0d0a  ent Learning},..
+00000bd0: 2020 6175 7468 6f72 3d7b 5975 616e 2c20    author={Yuan, 
+00000be0: 4d69 6e67 7169 2061 6e64 204c 756f 2c20  Mingqi and Luo, 
+00000bf0: 5368 6968 616f 2061 6e64 205a 6861 6e67  Shihao and Zhang
+00000c00: 2c20 5a65 7175 6e20 616e 6420 5961 6e67  , Zequn and Yang
+00000c10: 2c20 5875 2061 6e64 204a 696e 2c20 5869  , Xu and Jin, Xi
+00000c20: 6e20 616e 6420 4c69 2c20 426f 2061 6e64  n and Li, Bo and
+00000c30: 205a 656e 672c 2057 656e 6a75 6e7d 2c0d   Zeng, Wenjun},.
+00000c40: 0a20 206a 6f75 726e 616c 3d7b 6172 5869  .  journal={arXi
+00000c50: 7620 7072 6570 7269 6e74 2061 7258 6976  v preprint arXiv
+00000c60: 3a32 3331 312e 3135 3237 377d 2c0d 0a20  :2311.15277},.. 
+00000c70: 2079 6561 723d 7b32 3032 337d 0d0a 7d0d   year={2023}..}.
+00000c80: 0a60 6060 202d 2d3e                      .``` -->
```

### Comparing `hsuanwu-0.0.1b3/docs/license.md` & `hsuanwu-0.0.1b4/docs/license.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/mkgendocs.yml` & `hsuanwu-0.0.1b4/docs/mkgendocs.yml`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/contributing.md` & `hsuanwu-0.0.1b4/docs/contributing.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 To run tests with `pytest`:
 
 ```
 make pytest
 ```
 
-Type checking with `pytype` and `mypy`:
+Type checking with `pytype`:
 
 ```
 make type
 ```
 
 Codestyle check with `black`, `isort` and `ruff`:
```

### Comparing `hsuanwu-0.0.1b3/docs/api/index.md` & `hsuanwu-0.0.1b4/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/common/logger.md` & `hsuanwu-0.0.1b4/docs/api/common/logger.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/common/engine/__init__.md` & `hsuanwu-0.0.1b4/docs/api/common/engine/__init__.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/common/engine/base_policy_trainer.md` & `hsuanwu-0.0.1b4/docs/api/common/engine/base_policy_trainer.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/common/engine/distributed_trainer.md` & `hsuanwu-0.0.1b4/docs/api/common/engine/distributed_trainer.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/common/engine/off_policy_trainer.md` & `hsuanwu-0.0.1b4/docs/api/common/engine/off_policy_trainer.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/common/engine/on_policy_trainer.md` & `hsuanwu-0.0.1b4/docs/api/common/engine/on_policy_trainer.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/env/utils.md` & `hsuanwu-0.0.1b4/docs/api/env/utils.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/env/atari/__init__.md` & `hsuanwu-0.0.1b4/docs/api/env/atari/__init__.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/env/bullet/__init__.md` & `hsuanwu-0.0.1b4/docs/api/env/bullet/__init__.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/env/dmc/__init__.md` & `hsuanwu-0.0.1b4/docs/api/env/dmc/__init__.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/env/minigrid/__init__.md` & `hsuanwu-0.0.1b4/docs/api/env/minigrid/__init__.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/env/procgen/__init__.md` & `hsuanwu-0.0.1b4/docs/api/env/procgen/__init__.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/evaluation/comparison.md` & `hsuanwu-0.0.1b4/docs/api/evaluation/comparison.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/evaluation/performance.md` & `hsuanwu-0.0.1b4/docs/api/evaluation/performance.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/agent/base.md` & `hsuanwu-0.0.1b4/docs/api/xploit/agent/base.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/agent/drqv2.md` & `hsuanwu-0.0.1b4/docs/api/xploit/agent/drqv2.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/agent/impala.md` & `hsuanwu-0.0.1b4/docs/api/xploit/agent/impala.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/agent/ppg.md` & `hsuanwu-0.0.1b4/docs/api/xploit/agent/ppg.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/agent/ppo.md` & `hsuanwu-0.0.1b4/docs/api/xploit/agent/ppo.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/agent/sac.md` & `hsuanwu-0.0.1b4/docs/api/xploit/agent/sac.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/encoder/base.md` & `hsuanwu-0.0.1b4/docs/api/xploit/encoder/base.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/encoder/espeholt_residual_encoder.md` & `hsuanwu-0.0.1b4/docs/api/xploit/encoder/espeholt_residual_encoder.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/encoder/identity_encoder.md` & `hsuanwu-0.0.1b4/docs/api/xploit/encoder/identity_encoder.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/encoder/mnih_cnn_encoder.md` & `hsuanwu-0.0.1b4/docs/api/xploit/encoder/mnih_cnn_encoder.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/encoder/tassa_cnn_encoder.md` & `hsuanwu-0.0.1b4/docs/api/xploit/encoder/tassa_cnn_encoder.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/encoder/vanilla_mlp_encoder.md` & `hsuanwu-0.0.1b4/docs/api/xploit/encoder/vanilla_mlp_encoder.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/storage/distributed_storage.md` & `hsuanwu-0.0.1b4/docs/api/xploit/storage/distributed_storage.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/storage/nstep_replay_storage.md` & `hsuanwu-0.0.1b4/docs/api/xploit/storage/nstep_replay_storage.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/storage/prioritized_replay_storage.md` & `hsuanwu-0.0.1b4/docs/api/xploit/storage/prioritized_replay_storage.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/storage/vanilla_replay_storage.md` & `hsuanwu-0.0.1b4/docs/api/xploit/storage/vanilla_replay_storage.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xploit/storage/vanilla_rollout_storage.md` & `hsuanwu-0.0.1b4/docs/api/xploit/storage/vanilla_rollout_storage.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/auto_augment.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/auto_augment.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/elastic_transform.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/elastic_transform.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/gaussian_noise.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/gaussian_noise.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_adjustsharpness.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_adjustsharpness.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_amplitude_scaling.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_amplitude_scaling.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_autocontrast.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_autocontrast.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_colorjitter.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_colorjitter.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_convolution.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_convolution.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_crop.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_crop.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_cutout.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_cutout.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_cutoutcolor.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_cutoutcolor.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_equalize.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_equalize.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_flip.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_flip.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_invert.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_invert.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_perspective.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_perspective.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_rotate.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_rotate.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_shift.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_shift.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/augmentation/random_translate.md` & `hsuanwu-0.0.1b4/docs/api/xplore/augmentation/random_translate.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/distribution/base.md` & `hsuanwu-0.0.1b4/docs/api/xplore/distribution/base.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/distribution/categorical.md` & `hsuanwu-0.0.1b4/docs/api/xplore/distribution/categorical.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/distribution/diagonal_gaussian.md` & `hsuanwu-0.0.1b4/docs/api/xplore/distribution/diagonal_gaussian.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/distribution/normal_noise.md` & `hsuanwu-0.0.1b4/docs/api/xplore/distribution/normal_noise.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/distribution/ornstein_uhlenbeck_noise.md` & `hsuanwu-0.0.1b4/docs/api/xplore/distribution/ornstein_uhlenbeck_noise.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/distribution/squashed_normal.md` & `hsuanwu-0.0.1b4/docs/api/xplore/distribution/squashed_normal.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/distribution/truncated_normal_noise.md` & `hsuanwu-0.0.1b4/docs/api/xplore/distribution/truncated_normal_noise.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/reward/base.md` & `hsuanwu-0.0.1b4/docs/api/xplore/reward/base.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/reward/girm.md` & `hsuanwu-0.0.1b4/docs/api/xplore/reward/girm.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/reward/icm.md` & `hsuanwu-0.0.1b4/docs/api/xplore/reward/icm.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/reward/ngu.md` & `hsuanwu-0.0.1b4/docs/api/xplore/reward/ngu.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/reward/pseudo_counts.md` & `hsuanwu-0.0.1b4/docs/api/xplore/reward/pseudo_counts.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/reward/re3.md` & `hsuanwu-0.0.1b4/docs/api/xplore/reward/re3.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/reward/revd.md` & `hsuanwu-0.0.1b4/docs/api/xplore/reward/revd.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/reward/ride.md` & `hsuanwu-0.0.1b4/docs/api/xplore/reward/ride.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/reward/rise.md` & `hsuanwu-0.0.1b4/docs/api/xplore/reward/rise.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/api/xplore/reward/rnd.md` & `hsuanwu-0.0.1b4/docs/api/xplore/reward/rnd.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/assets/images/github_issues.png` & `hsuanwu-0.0.1b4/docs/assets/images/github_issues.png`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/assets/images/icon.svg` & `hsuanwu-0.0.1b4/docs/assets/images/icon.svg`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/assets/images/logo.png` & `hsuanwu-0.0.1b4/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/assets/images/qq.jpg` & `hsuanwu-0.0.1b4/docs/assets/images/qq.jpg`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/assets/images/rl_training.png` & `hsuanwu-0.0.1b4/docs/assets/images/rl_training.png`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/assets/images/roadmap.svg` & `hsuanwu-0.0.1b4/docs/assets/images/roadmap.svg`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/assets/images/slack.png` & `hsuanwu-0.0.1b4/docs/assets/images/slack.png`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/assets/images/structure.svg` & `hsuanwu-0.0.1b4/docs/assets/images/structure.svg`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/overview/api.md` & `hsuanwu-0.0.1b4/docs/overview/api.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/overview/env_index/index.md` & `hsuanwu-0.0.1b4/docs/overview/env_index/index.md`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/docs/overview/xploit_index/index.md` & `hsuanwu-0.0.1b4/docs/overview/xploit_index/index.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-+ **Encoder**: *Neural nework-based encoder for processing observations.*
-
-|Module|Input|Reference|Target Task|
-|:-|:-|:-|:-|
-|EspeholtResidualEncoder|Images|[IMPALA: Scalable Distributed Deep-RL with Importance Weighted Actor-Learner Architectures](http://proceedings.mlr.press/v80/espeholt18a/espeholt18a.pdf)|Atari or Procgen games.|
-|IdentityEncoder|States|N/A|DeepMind Control Suite: state|
-|MnihCnnEncoder|Images|[Playing Atari with Deep Reinforcement Learning](https://arxiv.org/pdf/1312.5602.pdf?source=post_page---------------------------)|Atari games.|
-|TassaCnnEncoder|Images|[DeepMind Control Suite](https://arxiv.org/pdf/1801.00690)|DeepMind Control Suite: pixel|
-|VanillaMlpEncoder|States|N/A|DeepMind Control Suite: state|
-
-> - **Naming Rule**: 'Surname of the first author' + 'Backbone' + 'Encoder'
-> - `Input`: Input type.
-> - `Target Task`: The testing tasks in their paper or potential tasks.
-
 + **Agent**: *Agent for interacting and learning.*
 
 |Module|Recurrent|Box|Discrete|MultiBinary|Multi Processing|NPU|Paper|Citations|
 |:-|:-|:-|:-|:-|:-|:-|:-|:-|
 |SAC|❌| ✔️ |❌|❌|❌|🐌 | [Link](http://proceedings.mlr.press/v80/haarnoja18b/haarnoja18b.pdf) |5077⭐|
 |DrQ|❌| ✔️ |❌|❌|❌|🐌 | [Link](https://arxiv.org/pdf/2004.13649) |433⭐|
 |DDPG|❌| ✔️ |❌|❌|❌|🐌 | [Link](https://arxiv.org/pdf/1509.02971.pdf?source=post_page---------------------------) |11819⭐|
 |DrQ-v2|❌| ✔️ |❌|❌|❌|🐌 | [Link](https://arxiv.org/pdf/2107.09645.pdf?utm_source=morioh.com) |100⭐|
 |PPO|❌| ✔️ |✔️|🐌|✔️|🐌 | [Link](https://arxiv.org/pdf/1707.06347) |11155⭐|
 |DrAC|❌| ✔️ |✔️|🐌|✔️|🐌 | [Link](https://proceedings.neurips.cc/paper/2021/file/2b38c2df6a49b97f706ec9148ce48d86-Paper.pdf) |29⭐|
 |PPG|❌| ✔️ |✔️|🐌|✔️|🐌| [Link](http://proceedings.mlr.press/v139/cobbe21a/cobbe21a.pdf) |82⭐|
 |IMPALA|✔️| ✔️ |✔️|🐌|✔️|🐌| [Link](http://proceedings.mlr.press/v80/espeholt18a/espeholt18a.pdf) |1219⭐|
 
-> - 🐌: Developing.
-> - `NPU`: Support Neural-network processing unit.
-> - `Recurrent`: Support recurrent neural network.
-> - `Box`: A N-dimensional box that containes every point in the action space.
-> - `Discrete`: A list of possible actions, where each timestep only one of the actions can be used.
-> - `MultiBinary`: A list of possible actions, where each timestep any of the actions can be used in any combination.
+!!! tip "Tips of Agent"
+    - 🐌: Developing.
+    - **NPU**: Support Neural-network processing unit.
+    - **Recurrent**: Support recurrent neural network.
+    - **Box**: A N-dimensional box that containes every point in the action space.
+    - **Discrete**: A list of possible actions, where each timestep only one of the actions can be used.
+    - **MultiBinary**: A list of possible actions, where each timestep any of the actions can be used in any combination.
+
++ **Encoder**: *Neural nework-based encoder for processing observations.*
+
+|Module|Input|Reference|Target Task|
+|:-|:-|:-|:-|
+|EspeholtResidualEncoder|Images|[IMPALA: Scalable Distributed Deep-RL with Importance Weighted Actor-Learner Architectures](http://proceedings.mlr.press/v80/espeholt18a/espeholt18a.pdf)|Atari or Procgen games.|
+|IdentityEncoder|States|N/A|DeepMind Control Suite: state|
+|MnihCnnEncoder|Images|[Playing Atari with Deep Reinforcement Learning](https://arxiv.org/pdf/1312.5602.pdf?source=post_page---------------------------)|Atari games.|
+|TassaCnnEncoder|Images|[DeepMind Control Suite](https://arxiv.org/pdf/1801.00690)|DeepMind Control Suite: pixel|
+|VanillaMlpEncoder|States|N/A|DeepMind Control Suite: state|
+
+!!! tip "Tips of Encoder"
+    - **Naming Rule**: 'Surname of the first author' + 'Backbone' + 'Encoder'
+    - **Input**: Input type.
+    - **Target Task**: The testing tasks in their paper or potential tasks.
 
 + **Storage**: *Storage for storing collected experiences.*
 
 |Module|Remark|
 |:-|:-|
 |VanillaRolloutStorage|On-Policy RL|
 |VanillaReplayStorage|Off-Policy RL|
```

### Comparing `hsuanwu-0.0.1b3/docs/overview/xplore_index/index.md` & `hsuanwu-0.0.1b4/docs/overview/xplore_index/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 | RIDE| Procedurally-generated environment | ✔️ |✔️| [RIDE: Rewarding Impact-Driven Exploration for Procedurally-Generated Environments](https://arxiv.org/pdf/2002.12292)|
 | RE3  | Entropy Maximization | ❌ |✔️| [State Entropy Maximization with Random Encoders for Efficient Exploration](http://proceedings.mlr.press/v139/seo21a/seo21a.pdf) |
 | RISE  | Entropy Maximization  | ❌  |✔️| [Rényi State Entropy Maximization for Exploration Acceleration in Reinforcement Learning](https://ieeexplore.ieee.org/abstract/document/9802917/) | 
 | REVD  | Divergence Maximization | ❌  |✔️| [Rewarding Episodic Visitation Discrepancy for Exploration in Reinforcement Learning](https://openreview.net/pdf?id=V2pw1VYMrDo)|
 |ProtoRL<sup>🐌</sup>| Entropy Maximization | ✔️ | ✔️ | [Reinforcement Learning with Prototypical Representations](http://proceedings.mlr.press/v139/yarats21a/yarats21a.pdf) |
 |APS<sup>🐌</sup>| Skill Discovery | ✔️ | ✔️ | [APS: Active Pretraining with Successor Features](http://proceedings.mlr.press/v139/liu21b/liu21b.pdf) |
 
-> - 🐌: Developing.
-> - `Repr.`: The method involves representation learning.
-> - `Visual`: The method works well in visual RL.
+!!! tip "Tips of Reward"
+    - **🐌**: Developing.
+    - **Repr.**: The method involves representation learning.
+    - **Visual**: The method works well in visual RL.
 
 + **Augmentation**: PyTorch.nn-like modules for observation augmentation.
 
 |Module|Input|Reference|
 |:-|:-|:-|
 |GaussianNoise|States| [Reinforcement Learning with Augmented Data](https://proceedings.neurips.cc/paper/2020/file/e615c82aba461681ade82da2da38004a-Paper.pdf) |
 |RandomAmplitudeScaling|States|[Reinforcement Learning with Augmented Data](https://proceedings.neurips.cc/paper/2020/file/e615c82aba461681ade82da2da38004a-Paper.pdf) |
@@ -50,8 +51,9 @@
 |NormalNoise|Noise|[torch.distributions](https://pytorch.org/docs/stable/distributions.html)|
 |OrnsteinUhlenbeckNoise|Noise|[Continuous Control with Deep Reinforcement Learning](https://arxiv.org/pdf/1509.02971.pdf?source=post_page---------------------------)|
 |TruncatedNormalNoise|Noise|[Mastering Visual Continuous Control: Improved Data-Augmented Reinforcement Learning](https://arxiv.org/pdf/2107.09645.pdf?utm_source=morioh.com)|
 |Categorical|Distribution|[torch.distributions](https://pytorch.org/docs/stable/distributions.html)|
 |DiagonalGaussian|Distribution|[torch.distributions](https://pytorch.org/docs/stable/distributions.html)|
 |SquashedNormal|Distribution|[torch.distributions](https://pytorch.org/docs/stable/distributions.html)|
 
-> - In Hsuanwu, the action noise is implemented via a `Distribution` manner to realize unification.
+!!! tip "Tips of Distribution"
+  - In Hsuanwu, the action noise is implemented via a `Distribution` manner to realize unification.
```

### Comparing `hsuanwu-0.0.1b3/hsuanwu/common/logger.py` & `hsuanwu-0.0.1b4/hsuanwu/common/logger.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/common/engine/__init__.py` & `hsuanwu-0.0.1b4/hsuanwu/common/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/common/engine/base_policy_trainer.py` & `hsuanwu-0.0.1b4/hsuanwu/common/engine/base_policy_trainer.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/common/engine/distributed_trainer.py` & `hsuanwu-0.0.1b4/hsuanwu/common/engine/distributed_trainer.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/common/engine/off_policy_trainer.py` & `hsuanwu-0.0.1b4/hsuanwu/common/engine/off_policy_trainer.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/common/engine/on_policy_trainer.py` & `hsuanwu-0.0.1b4/hsuanwu/common/engine/on_policy_trainer.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/env/utils.py` & `hsuanwu-0.0.1b4/hsuanwu/env/utils.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/env/atari/__init__.py` & `hsuanwu-0.0.1b4/hsuanwu/env/atari/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/env/atari/wrappers.py` & `hsuanwu-0.0.1b4/hsuanwu/env/atari/wrappers.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/env/bullet/__init__.py` & `hsuanwu-0.0.1b4/hsuanwu/env/bullet/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/env/dmc/__init__.py` & `hsuanwu-0.0.1b4/hsuanwu/env/dmc/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/env/dmc/natural_imgsource.py` & `hsuanwu-0.0.1b4/hsuanwu/env/dmc/natural_imgsource.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/env/dmc/wrappers.py` & `hsuanwu-0.0.1b4/hsuanwu/env/dmc/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         info["discount"] = time_step.discount
         info["step_type"] = time_step.step_type
         if done and time_step.discount == 1.0:
             truncated = True
         else:
             truncated = False
 
-        terminated = False
+        terminated = truncated
         return obs, reward, terminated, truncated, info
 
     def reset(self, **kwargs) -> Tuple[np.ndarray, Dict]:
         time_step = self._env.reset()
         obs = self._get_obs(time_step)
         return obs, {}
```

### Comparing `hsuanwu-0.0.1b3/hsuanwu/env/minigrid/__init__.py` & `hsuanwu-0.0.1b4/hsuanwu/env/minigrid/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/env/procgen/__init__.py` & `hsuanwu-0.0.1b4/hsuanwu/env/procgen/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/evaluation/comparison.py` & `hsuanwu-0.0.1b4/hsuanwu/evaluation/comparison.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/evaluation/performance.py` & `hsuanwu-0.0.1b4/hsuanwu/evaluation/performance.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/evaluation/utils.py` & `hsuanwu-0.0.1b4/hsuanwu/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/experimental/npu_ppo.py` & `hsuanwu-0.0.1b4/hsuanwu/experimental/npu_ppo.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/agent/__init__.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/agent/base.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/base.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/agent/drqv2.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/drqv2.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/agent/impala.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/impala.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/agent/network.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/network.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/agent/ppg.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/ppg.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/agent/ppo.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/ppo.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/agent/sac.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/sac.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/agent/utils.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/agent/utils.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/base.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/base.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/espeholt_residual_encoder.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/espeholt_residual_encoder.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/identity_encoder.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/identity_encoder.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/mnih_cnn_encoder.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/mnih_cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/tassa_cnn_encoder.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/tassa_cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/encoder/vanilla_mlp_encoder.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/encoder/vanilla_mlp_encoder.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/storage/base.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/base.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/storage/distributed_storage.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/distributed_storage.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/storage/nstep_replay_storage.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/nstep_replay_storage.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/storage/prioritized_replay_storage.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/prioritized_replay_storage.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/storage/utils.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/utils.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/storage/vanilla_replay_storage.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/vanilla_replay_storage.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xploit/storage/vanilla_rollout_storage.py` & `hsuanwu-0.0.1b4/hsuanwu/xploit/storage/vanilla_rollout_storage.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/__init__.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/auto_augment.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/auto_augment.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/elastic_transform.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/elastic_transform.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/gaussian_noise.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/grayscale.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/grayscale.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_adjustsharpness.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_adjustsharpness.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_amplitude_scaling.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_amplitude_scaling.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_augment.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_augment.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_autocontrast.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_autocontrast.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_colorjitter.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_colorjitter.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_convolution.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_convolution.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_crop.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_crop.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_cutout.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_cutout.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_cutoutcolor.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_cutoutcolor.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_equalize.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_equalize.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_flip.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_flip.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_invert.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_invert.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_perspective.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_perspective.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_rotate.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_rotate.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_shift.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_shift.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/augmentation/random_translate.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/augmentation/random_translate.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/__init__.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/base.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/base.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/categorical.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/categorical.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/diagonal_gaussian.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/diagonal_gaussian.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/normal_noise.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/normal_noise.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/ornstein_uhlenbeck_noise.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/squashed_normal.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/squashed_normal.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/truncated_normal_noise.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/truncated_normal_noise.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/distribution/utils.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/distribution/utils.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/__init__.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/__init__.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/base.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/base.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/girm.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/girm.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/icm.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/icm.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/ngu.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/ngu.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/pseudo_counts.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/pseudo_counts.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/re3.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/re3.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/revd.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/revd.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/ride.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/ride.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/rise.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/rise.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/hsuanwu/xplore/reward/rnd.py` & `hsuanwu-0.0.1b4/hsuanwu/xplore/reward/rnd.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/tests/test_aug.py` & `hsuanwu-0.0.1b4/tests/test_aug.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/tests/test_dist.py` & `hsuanwu-0.0.1b4/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/tests/test_env.py` & `hsuanwu-0.0.1b4/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/tests/test_eval.py` & `hsuanwu-0.0.1b4/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/tests/test_logger.py` & `hsuanwu-0.0.1b4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/tests/test_mp.py` & `hsuanwu-0.0.1b4/tests/test_mp.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/tests/test_reward.py` & `hsuanwu-0.0.1b4/tests/test_reward.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/tests/test_torch.py` & `hsuanwu-0.0.1b4/tests/test_torch.py`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/LICENSE` & `hsuanwu-0.0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `hsuanwu-0.0.1b3/README.md` & `hsuanwu-0.0.1b4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 - 🚀 Optimized workflow for full hardware acceleration;
 - ⚙️ Support for custom environments;
 - 🖥️ Support for multiple computing devices like GPU and NPU;
 - 🛠️ Support for RL model engineering deployment (TensorRT, CANN, ...);
 - 💾 Large number of reusable bechmarks ([See HsuanwuHub](hub.hsuanwu.dev));
 - 📋 Elegant experimental management powered by [Hydra](https://hydra.cc/).
 
-Join the development community for issues and discussions:
+Join the developer community for issues and discussions:
 |Slack|QQ|GitHub|
 |:-:|:-:|:-:|
 |<a href="https://app.slack.com/client/T054J4NJXP0/C054T78QZ9A"><img src='./docs/assets/images/slack.png' style="width: 50%" ></a>|<img src='./docs/assets/images/qq.jpg' style="width: 65%">|<a href="https://github.com/RLE-Foundation/Hsuanwu/issues"><img src='./docs/assets/images/github_issues.png' style="width: 50%"></a>|
 
 
 
 <!-- Please cite the following paper if you use Hsuanwu in your work, thank you!
@@ -44,14 +44,16 @@
 - [Model Zoo](#model-zoo)
 - [API Documentation](#api-documentation)
 - [How To Contribute](#how-to-contribute)
 - [Acknowledgment](#acknowledgment)
 
 # Quick Start
 ## Installation
+- Prerequisites
+
 Currently, Hsuanwu requires `Python>=3.8`, user can create an virtual environment by
 ``` sh
 conda create -n hsuanwu python=3.8
 ```
 
 - with pip `recommended`
```

#### html2text {}

```diff
@@ -18,51 +18,52 @@
 deployment, etc. The highlight features of Hsuanwu: - â±ï¸ Latest algorithms
 and tricks; - ð§± Highly modularized design for complete decoupling of RL
 algorithms; - ð Optimized workflow for full hardware acceleration; - âï¸
 Support for custom environments; - ð¥ï¸ Support for multiple computing
 devices like GPU and NPU; - ð ï¸ Support for RL model engineering deployment
 (TensorRT, CANN, ...); - ð¾ Large number of reusable bechmarks ([See
 HsuanwuHub](hub.hsuanwu.dev)); - ð Elegant experimental management powered
-by [Hydra](https://hydra.cc/). Join the development community for issues and
+by [Hydra](https://hydra.cc/). Join the developer community for issues and
 discussions: |Slack|QQ|GitHub| |:-:|:-:|:-:| |[./docs/assets/images/slack.png]|
 [./docs/assets/images/qq.jpg]|[./docs/assets/images/github_issues.png]|  -
 [Quick Start](#quick-start) - [Installation](#installation) - [Build your first
 Hsuanwu application](#build-your-first-hsuanwu-application) - [Implemented
 Modules](#implemented-modules) - [Roadmap](#roadmap) - [Project Structure]
 (#project-structure) - [RL Agents](#rl-agents) - [Intrinsic Reward Modules]
 (#intrinsic-reward-modules) - [Model Zoo](#model-zoo) - [API Documentation]
 (#api-documentation) - [How To Contribute](#how-to-contribute) -
-[Acknowledgment](#acknowledgment) # Quick Start ## Installation Currently,
-Hsuanwu requires `Python>=3.8`, user can create an virtual environment by ```
-sh conda create -n hsuanwu python=3.8 ``` - with pip `recommended` Open up a
-terminal and install **Hsuanwu** with `pip`: ``` shell pip install hsuanwu #
-basic installation pip install hsuanwu[envs] # for pre-defined environments pip
-install hsuanwu[tests] # for project tests pip install hsuanwu[all] # install
-all the dependencies ``` - with git Open up a terminal and clone the repository
-from [GitHub](https://github.com/RLE-Foundation/Hsuanwu) with `git`: ``` sh git
-clone https://github.com/RLE-Foundation/Hsuanwu.git ``` After that, run the
-following command to install package and dependencies: ``` sh pip install -e .
-# basic installation pip install -e .[envs] # for pre-defined environments pip
-install -e .[tests] # for project tests pip install -e .[all] # install all the
-dependencies ``` For more detailed installation instruction, see [https://
-docs.hsuanwu.dev/getting_started](https://docs.hsuanwu.dev/getting_started). ##
-Build your first Hsuanwu application For example, we want to use [DrQ-v2]
-(https://openreview.net/forum?id=_SJ-_yyes8) to solve a task of [DeepMind
-Control Suite](https://github.com/deepmind/dm_control), and we only need the
-following two steps: 1. Write a `config.yaml` file in your working directory
-like: ``` yaml experiment: drqv2_dmc # Experiment ID. device: cuda:0 # Device
-(cpu, cuda, ...) on which the code should be run. seed: 1 # Random seed for
-reproduction. num_train_steps: 250000 # Number of training steps. agent: name:
-DrQv2 # The agent name. ``` 2. Write a `train.py` file like: ``` python import
-hydra # Use Hydra to manage experiments from hsuanwu.env import make_dmc_env #
-Import DeepMind Control Suite from hsuanwu.common.engine import HsuanwuEngine #
-Import Hsuanwu engine train_env = make_dmc_env(env_id='cartpole_balance') #
-Create train env test_env = make_dmc_env(env_id='cartpole_balance') # Create
-test env @hydra.main(version_base=None, config_path='./', config_name='config')
-def main(cfgs): engine = HsuanwuEngine(cfgs=cfgs, train_env=train_env,
+[Acknowledgment](#acknowledgment) # Quick Start ## Installation - Prerequisites
+Currently, Hsuanwu requires `Python>=3.8`, user can create an virtual
+environment by ``` sh conda create -n hsuanwu python=3.8 ``` - with pip
+`recommended` Open up a terminal and install **Hsuanwu** with `pip`: ``` shell
+pip install hsuanwu # basic installation pip install hsuanwu[envs] # for pre-
+defined environments pip install hsuanwu[tests] # for project tests pip install
+hsuanwu[all] # install all the dependencies ``` - with git Open up a terminal
+and clone the repository from [GitHub](https://github.com/RLE-Foundation/
+Hsuanwu) with `git`: ``` sh git clone https://github.com/RLE-Foundation/
+Hsuanwu.git ``` After that, run the following command to install package and
+dependencies: ``` sh pip install -e . # basic installation pip install -e .
+[envs] # for pre-defined environments pip install -e .[tests] # for project
+tests pip install -e .[all] # install all the dependencies ``` For more
+detailed installation instruction, see [https://docs.hsuanwu.dev/
+getting_started](https://docs.hsuanwu.dev/getting_started). ## Build your first
+Hsuanwu application For example, we want to use [DrQ-v2](https://
+openreview.net/forum?id=_SJ-_yyes8) to solve a task of [DeepMind Control Suite]
+(https://github.com/deepmind/dm_control), and we only need the following two
+steps: 1. Write a `config.yaml` file in your working directory like: ``` yaml
+experiment: drqv2_dmc # Experiment ID. device: cuda:0 # Device (cpu, cuda, ...)
+on which the code should be run. seed: 1 # Random seed for reproduction.
+num_train_steps: 250000 # Number of training steps. agent: name: DrQv2 # The
+agent name. ``` 2. Write a `train.py` file like: ``` python import hydra # Use
+Hydra to manage experiments from hsuanwu.env import make_dmc_env # Import
+DeepMind Control Suite from hsuanwu.common.engine import HsuanwuEngine # Import
+Hsuanwu engine train_env = make_dmc_env(env_id='cartpole_balance') # Create
+train env test_env = make_dmc_env(env_id='cartpole_balance') # Create test env
+@hydra.main(version_base=None, config_path='./', config_name='config') def main
+(cfgs): engine = HsuanwuEngine(cfgs=cfgs, train_env=train_env,
 test_env=test_env) # Initialize engine engine.invoke() # Start training if
 __name__ == '__main__': main() ``` Run `train.py` and you will see the
 following output:
                     [./docs/assets/images/rl_training.png]
 For more detailed tutorials, see [https://docs.hsuanwu.dev/tutorials](https://
 docs.hsuanwu.dev/tutorials). # Implemented Modules ## Roadmap Hsuanwu evolves
 based on reinforcement learning algorithms and integrates latest tricks. The
```

### Comparing `hsuanwu-0.0.1b3/pyproject.toml` & `hsuanwu-0.0.1b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hsuanwu"
-version = "0.0.1.beta03"
+version = "0.0.1.beta04"
 authors = [
   { name="Reinforcement Learning Evolution Foundation", email="friedrichyuan19990827@gmail.com" },
 ]
 description = "Long-Term Evolution Project of Reinforcement Learning"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["Reinforcement Learning", "Algorithm", "Evolution", "Baseline"]
```

### Comparing `hsuanwu-0.0.1b3/PKG-INFO` & `hsuanwu-0.0.1b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsuanwu
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: Long-Term Evolution Project of Reinforcement Learning
 Project-URL: Code, https://github.com/RLE-Foundation/Hsuanwu
 Project-URL: Documentation, https://docs.hsuanwu.dev/
 Project-URL: Benchmark, https://hub.hsuanwu.dev/
 Project-URL: Bug Tracker, https://github.com/RLE-Foundation/Hsuanwu/issues
 Author-email: Reinforcement Learning Evolution Foundation <friedrichyuan19990827@gmail.com>
 License-File: LICENSE
@@ -62,15 +62,15 @@
 - 🚀 Optimized workflow for full hardware acceleration;
 - ⚙️ Support for custom environments;
 - 🖥️ Support for multiple computing devices like GPU and NPU;
 - 🛠️ Support for RL model engineering deployment (TensorRT, CANN, ...);
 - 💾 Large number of reusable bechmarks ([See HsuanwuHub](hub.hsuanwu.dev));
 - 📋 Elegant experimental management powered by [Hydra](https://hydra.cc/).
 
-Join the development community for issues and discussions:
+Join the developer community for issues and discussions:
 |Slack|QQ|GitHub|
 |:-:|:-:|:-:|
 |<a href="https://app.slack.com/client/T054J4NJXP0/C054T78QZ9A"><img src='./docs/assets/images/slack.png' style="width: 50%" ></a>|<img src='./docs/assets/images/qq.jpg' style="width: 65%">|<a href="https://github.com/RLE-Foundation/Hsuanwu/issues"><img src='./docs/assets/images/github_issues.png' style="width: 50%"></a>|
 
 
 
 <!-- Please cite the following paper if you use Hsuanwu in your work, thank you!
@@ -94,14 +94,16 @@
 - [Model Zoo](#model-zoo)
 - [API Documentation](#api-documentation)
 - [How To Contribute](#how-to-contribute)
 - [Acknowledgment](#acknowledgment)
 
 # Quick Start
 ## Installation
+- Prerequisites
+
 Currently, Hsuanwu requires `Python>=3.8`, user can create an virtual environment by
 ``` sh
 conda create -n hsuanwu python=3.8
 ```
 
 - with pip `recommended`
```


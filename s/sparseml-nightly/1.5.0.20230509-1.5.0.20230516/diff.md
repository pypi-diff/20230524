# Comparing `tmp/sparseml_nightly-1.5.0.20230509-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.5.0.20230516-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,370 +1,370 @@
-Zip file size: 945872 bytes, number of entries: 368
--rw-rw-r--  2.0 unx     1413 b- defN 23-May-09 03:01 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-May-09 03:01 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-May-09 03:01 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-May-09 03:01 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-May-09 03:01 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-May-09 03:01 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17631 b- defN 23-May-09 03:01 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-May-09 03:01 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-May-09 03:01 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-May-09 03:01 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-May-09 03:01 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-May-09 03:01 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-May-09 03:01 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-May-09 03:01 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-May-09 03:01 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-May-09 03:01 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     4751 b- defN 23-May-09 03:01 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2252 b- defN 23-May-09 03:01 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-May-09 03:01 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-May-09 03:01 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-May-09 03:01 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-May-09 03:01 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-May-09 03:01 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-May-09 03:01 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-May-09 03:01 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-May-09 03:01 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-May-09 03:01 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-May-09 03:01 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-May-09 03:01 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-May-09 03:01 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-May-09 03:01 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4470 b- defN 23-May-09 03:01 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4571 b- defN 23-May-09 03:01 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-May-09 03:01 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-May-09 03:01 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-May-09 03:01 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-May-09 03:01 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-May-09 03:01 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-May-09 03:01 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-May-09 03:01 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-May-09 03:01 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-May-09 03:01 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      730 b- defN 23-May-09 03:01 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx     8704 b- defN 23-May-09 03:01 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-May-09 03:01 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-May-09 03:01 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-May-09 03:01 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-May-09 03:01 sparseml/framework/info.py
--rw-rw-r--  2.0 unx      970 b- defN 23-May-09 03:01 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-May-09 03:01 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-May-09 03:01 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-May-09 03:01 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-May-09 03:01 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-May-09 03:01 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-May-09 03:01 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-May-09 03:01 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-May-09 03:01 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-May-09 03:01 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-May-09 03:01 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-May-09 03:01 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-May-09 03:01 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-May-09 03:01 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-May-09 03:01 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-May-09 03:01 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-May-09 03:01 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-May-09 03:01 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-May-09 03:01 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-May-09 03:01 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-May-09 03:01 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-May-09 03:01 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-May-09 03:01 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-May-09 03:01 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-May-09 03:01 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-May-09 03:01 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-May-09 03:01 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-May-09 03:01 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-May-09 03:01 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-May-09 03:01 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-May-09 03:01 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-May-09 03:01 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-May-09 03:01 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-May-09 03:01 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-May-09 03:01 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-May-09 03:01 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-May-09 03:01 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-May-09 03:01 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-May-09 03:01 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-May-09 03:01 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-May-09 03:01 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-May-09 03:01 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-May-09 03:01 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13274 b- defN 23-May-09 03:01 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19634 b- defN 23-May-09 03:01 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-May-09 03:01 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-May-09 03:01 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14520 b- defN 23-May-09 03:01 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-May-09 03:01 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4514 b- defN 23-May-09 03:01 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-May-09 03:01 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-May-09 03:01 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-May-09 03:01 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-May-09 03:01 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-May-09 03:01 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13002 b- defN 23-May-09 03:01 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    16407 b- defN 23-May-09 03:01 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-May-09 03:01 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    41529 b- defN 23-May-09 03:01 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-May-09 03:01 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31586 b- defN 23-May-09 03:01 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-May-09 03:01 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      734 b- defN 23-May-09 03:01 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3694 b- defN 23-May-09 03:01 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-May-09 03:01 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-May-09 03:01 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-May-09 03:01 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-May-09 03:01 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-May-09 03:01 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-May-09 03:01 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-May-09 03:01 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-May-09 03:01 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     1848 b- defN 23-May-09 03:01 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6173 b- defN 23-May-09 03:01 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-May-09 03:01 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10826 b- defN 23-May-09 03:01 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     2814 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-May-09 03:01 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-May-09 03:01 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-May-09 03:01 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    20912 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-May-09 03:01 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-May-09 03:01 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-May-09 03:01 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-May-09 03:01 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-May-09 03:01 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-May-09 03:01 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-May-09 03:01 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-May-09 03:01 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-May-09 03:01 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-May-09 03:01 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-May-09 03:01 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-May-09 03:01 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-May-09 03:01 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-May-09 03:01 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-May-09 03:01 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-May-09 03:01 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-May-09 03:01 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-May-09 03:01 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-May-09 03:01 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-May-09 03:01 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-May-09 03:01 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-May-09 03:01 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-May-09 03:01 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-May-09 03:01 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-May-09 03:01 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-May-09 03:01 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-May-09 03:01 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-May-09 03:01 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-May-09 03:01 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26253 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17591 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    69959 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-May-09 03:01 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      744 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-May-09 03:01 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-May-09 03:01 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-May-09 03:01 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-May-09 03:01 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-May-09 03:01 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31056 b- defN 23-May-09 03:01 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    39284 b- defN 23-May-09 03:01 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-May-09 03:01 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-May-09 03:01 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-May-09 03:01 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-May-09 03:01 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-May-09 03:01 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-May-09 03:01 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-May-09 03:01 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-May-09 03:01 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-May-09 03:01 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-May-09 03:01 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-May-09 03:01 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-May-09 03:01 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-May-09 03:01 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-May-09 03:01 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-May-09 03:01 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-May-09 03:01 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-May-09 03:01 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-May-09 03:01 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-May-09 03:01 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-May-09 03:01 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-May-09 03:01 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-May-09 03:01 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-May-09 03:01 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-May-09 03:01 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-May-09 03:01 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-May-09 03:01 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx      987 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-May-09 03:01 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-May-09 03:01 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    19731 b- defN 23-May-09 03:01 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30936 b- defN 23-May-09 03:01 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36738 b- defN 23-May-09 03:01 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40480 b- defN 23-May-09 03:01 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34530 b- defN 23-May-09 03:01 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-May-09 03:01 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-May-09 03:01 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    43756 b- defN 23-May-09 03:01 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-May-09 03:01 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-May-09 03:01 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-May-09 03:01 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-May-09 03:01 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    15797 b- defN 23-May-09 03:01 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-May-09 03:01 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-May-09 03:01 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26321 b- defN 23-May-09 03:01 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-May-09 03:01 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-May-09 03:01 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-May-09 03:01 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-May-09 03:01 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-May-09 03:01 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-May-09 03:01 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-May-09 03:01 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-May-09 03:01 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-May-09 03:01 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-May-09 03:01 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-May-09 03:01 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-May-09 03:01 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-May-09 03:01 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-May-09 03:01 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-May-09 03:01 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1245 b- defN 23-May-09 03:01 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-May-09 03:01 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-May-09 03:01 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-May-09 03:01 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx      958 b- defN 23-May-09 03:01 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-May-09 03:01 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-May-09 03:01 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-May-09 03:01 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-May-09 03:01 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    34223 b- defN 23-May-09 03:01 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2666 b- defN 23-May-09 03:01 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-May-09 03:01 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-May-09 03:01 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6288 b- defN 23-May-09 03:01 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-May-09 03:01 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21295 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2372 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    36575 b- defN 23-May-09 03:03 sparseml_nightly-1.5.0.20230509.dist-info/RECORD
-368 files, 3423373 bytes uncompressed, 886664 bytes compressed:  74.1%
+Zip file size: 945452 bytes, number of entries: 368
+-rw-rw-r--  2.0 unx     1413 b- defN 23-May-16 03:01 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-May-16 03:01 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-May-16 03:01 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-May-16 03:01 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-May-16 03:01 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-May-16 03:01 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17631 b- defN 23-May-16 03:01 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-May-16 03:01 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-May-16 03:01 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-May-16 03:01 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-May-16 03:01 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-May-16 03:01 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-May-16 03:01 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-May-16 03:01 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-May-16 03:01 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-May-16 03:01 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     4783 b- defN 23-May-16 03:01 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2252 b- defN 23-May-16 03:01 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-May-16 03:01 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-May-16 03:01 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     3866 b- defN 23-May-16 03:01 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-May-16 03:01 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-May-16 03:01 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-May-16 03:01 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-May-16 03:01 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-May-16 03:01 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-May-16 03:01 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-May-16 03:01 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-May-16 03:01 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-May-16 03:01 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-May-16 03:01 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     4470 b- defN 23-May-16 03:01 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4571 b- defN 23-May-16 03:01 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-May-16 03:01 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-May-16 03:01 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3398 b- defN 23-May-16 03:01 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-May-16 03:01 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-May-16 03:01 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-May-16 03:01 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-May-16 03:01 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-May-16 03:01 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-May-16 03:01 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-May-16 03:01 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx     8704 b- defN 23-May-16 03:01 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-May-16 03:01 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-May-16 03:01 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-May-16 03:01 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-May-16 03:01 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx      970 b- defN 23-May-16 03:01 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-May-16 03:01 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-May-16 03:01 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-May-16 03:01 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-May-16 03:01 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-May-16 03:01 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-May-16 03:01 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-May-16 03:01 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-May-16 03:01 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-May-16 03:01 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-May-16 03:01 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-May-16 03:01 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-May-16 03:01 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-May-16 03:01 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-May-16 03:01 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-May-16 03:01 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-May-16 03:01 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-May-16 03:01 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-May-16 03:01 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-May-16 03:01 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-May-16 03:01 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-May-16 03:01 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-May-16 03:01 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-May-16 03:01 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-May-16 03:01 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-May-16 03:01 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-May-16 03:01 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-May-16 03:01 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-May-16 03:01 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-May-16 03:01 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-May-16 03:01 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-May-16 03:01 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-May-16 03:01 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-May-16 03:01 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-May-16 03:01 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-May-16 03:01 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-May-16 03:01 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-May-16 03:01 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-May-16 03:01 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-May-16 03:01 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-May-16 03:01 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-May-16 03:01 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-May-16 03:01 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13285 b- defN 23-May-16 03:01 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19639 b- defN 23-May-16 03:01 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-May-16 03:01 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-May-16 03:01 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14532 b- defN 23-May-16 03:01 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-May-16 03:01 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4552 b- defN 23-May-16 03:01 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-May-16 03:01 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-May-16 03:01 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-May-16 03:01 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-May-16 03:01 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-May-16 03:01 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-May-16 03:01 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    16407 b- defN 23-May-16 03:01 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-May-16 03:01 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    40230 b- defN 23-May-16 03:01 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-May-16 03:01 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31591 b- defN 23-May-16 03:01 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-May-16 03:01 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      734 b- defN 23-May-16 03:01 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-May-16 03:01 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-May-16 03:01 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-May-16 03:01 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-May-16 03:01 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-May-16 03:01 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-May-16 03:01 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-May-16 03:01 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-May-16 03:01 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-May-16 03:01 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     1848 b- defN 23-May-16 03:01 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6173 b- defN 23-May-16 03:01 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-May-16 03:01 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10864 b- defN 23-May-16 03:01 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     2814 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4017 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-May-16 03:01 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-May-16 03:01 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-May-16 03:01 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-May-16 03:01 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-May-16 03:01 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-May-16 03:01 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-May-16 03:01 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-May-16 03:01 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-May-16 03:01 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-May-16 03:01 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-May-16 03:01 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    20912 b- defN 23-May-16 03:01 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-May-16 03:01 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-May-16 03:01 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-May-16 03:01 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-May-16 03:01 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-May-16 03:01 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-May-16 03:01 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-May-16 03:01 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-May-16 03:01 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-May-16 03:01 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-May-16 03:01 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-May-16 03:01 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-May-16 03:01 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-May-16 03:01 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-May-16 03:01 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-May-16 03:01 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-May-16 03:01 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-May-16 03:01 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-May-16 03:01 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-May-16 03:01 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-May-16 03:01 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-May-16 03:01 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-May-16 03:01 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-May-16 03:01 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-May-16 03:01 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-May-16 03:01 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-May-16 03:01 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-May-16 03:01 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-May-16 03:01 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-May-16 03:01 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-May-16 03:01 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-May-16 03:01 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-May-16 03:01 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-May-16 03:01 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-May-16 03:01 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-May-16 03:01 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-May-16 03:01 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-May-16 03:01 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-May-16 03:01 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-May-16 03:01 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-May-16 03:01 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-May-16 03:01 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-May-16 03:01 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26253 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17591 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    69997 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-May-16 03:01 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      744 b- defN 23-May-16 03:01 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-May-16 03:01 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-May-16 03:01 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-May-16 03:01 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-May-16 03:01 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-May-16 03:01 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-May-16 03:01 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-May-16 03:01 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-May-16 03:01 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-May-16 03:01 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-May-16 03:01 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31098 b- defN 23-May-16 03:01 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-May-16 03:01 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-May-16 03:01 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-May-16 03:01 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-May-16 03:01 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-May-16 03:01 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-May-16 03:01 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-May-16 03:01 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-May-16 03:01 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-May-16 03:01 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-May-16 03:01 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-May-16 03:01 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-May-16 03:01 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-May-16 03:01 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-May-16 03:01 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-May-16 03:01 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-May-16 03:01 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-May-16 03:01 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-May-16 03:01 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-May-16 03:01 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-May-16 03:01 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-May-16 03:01 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-May-16 03:01 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-May-16 03:01 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-May-16 03:01 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-May-16 03:01 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-May-16 03:01 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-May-16 03:01 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx      987 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-May-16 03:01 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-May-16 03:01 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    20377 b- defN 23-May-16 03:01 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-May-16 03:01 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36557 b- defN 23-May-16 03:01 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40299 b- defN 23-May-16 03:01 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34350 b- defN 23-May-16 03:01 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-May-16 03:01 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-May-16 03:01 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    43756 b- defN 23-May-16 03:01 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-May-16 03:01 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-May-16 03:01 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-May-16 03:01 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-May-16 03:01 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    15797 b- defN 23-May-16 03:01 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-May-16 03:01 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-May-16 03:01 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26321 b- defN 23-May-16 03:01 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-May-16 03:01 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-May-16 03:01 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-May-16 03:01 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-May-16 03:01 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-May-16 03:01 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-May-16 03:01 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-May-16 03:01 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-May-16 03:01 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-May-16 03:01 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-May-16 03:01 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-May-16 03:01 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-May-16 03:01 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-May-16 03:01 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-May-16 03:01 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-May-16 03:01 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1245 b- defN 23-May-16 03:01 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-May-16 03:01 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-May-16 03:01 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-May-16 03:01 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx      958 b- defN 23-May-16 03:01 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-May-16 03:01 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-May-16 03:01 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-May-16 03:01 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-May-16 03:01 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    34242 b- defN 23-May-16 03:01 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2666 b- defN 23-May-16 03:01 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-May-16 03:01 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-May-16 03:01 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6288 b- defN 23-May-16 03:01 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-May-16 03:01 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-May-16 03:03 sparseml_nightly-1.5.0.20230516.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21292 b- defN 23-May-16 03:03 sparseml_nightly-1.5.0.20230516.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-May-16 03:03 sparseml_nightly-1.5.0.20230516.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-16 03:03 sparseml_nightly-1.5.0.20230516.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2372 b- defN 23-May-16 03:03 sparseml_nightly-1.5.0.20230516.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-16 03:03 sparseml_nightly-1.5.0.20230516.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    36575 b- defN 23-May-16 03:03 sparseml_nightly-1.5.0.20230516.dist-info/RECORD
+368 files, 3422265 bytes uncompressed, 886244 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -1077,29 +1077,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230509.dist-info/LICENSE
+Filename: sparseml_nightly-1.5.0.20230516.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230509.dist-info/METADATA
+Filename: sparseml_nightly-1.5.0.20230516.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230509.dist-info/NOTICE
+Filename: sparseml_nightly-1.5.0.20230516.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230509.dist-info/WHEEL
+Filename: sparseml_nightly-1.5.0.20230516.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230509.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.5.0.20230516.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230509.dist-info/top_level.txt
+Filename: sparseml_nightly-1.5.0.20230516.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.5.0.20230509.dist-info/RECORD
+Filename: sparseml_nightly-1.5.0.20230516.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/exporters/onnx_to_deepsparse.py

```diff
@@ -17,14 +17,15 @@
 from pathlib import Path
 from typing import Union
 
 import onnx
 
 from sparseml.exporters import transforms as sparseml_transforms
 from sparseml.exporters.base_exporter import BaseExporter
+from sparsezoo import save_onnx
 
 
 class ONNXToDeepsparse(BaseExporter):
     """
     Optimizes an `onnx.ModelProto` for the deepsparse engine by applying a
     series of transformations to a onnx graph with quantize operations.
 
@@ -105,11 +106,11 @@
         # sanity check
         if not isinstance(model, onnx.ModelProto):
             raise TypeError(f"Expected onnx.ModelProto, found {type(model)}")
         return model
 
     def export(self, pre_transforms_model: onnx.ModelProto, file_path: str):
         if self.export_input_model or os.getenv("SAVE_PREQAT_ONNX", False):
-            onnx.save(pre_transforms_model, file_path.replace(".onnx", ".preqat.onnx"))
+            save_onnx(pre_transforms_model, file_path.replace(".onnx", ".preqat.onnx"))
 
         post_transforms_model: onnx.ModelProto = self.apply(pre_transforms_model)
-        onnx.save(post_transforms_model, file_path)
+        save_onnx(post_transforms_model, file_path)
```

## sparseml/exporters/transforms/onnx_transform.py

```diff
@@ -16,15 +16,16 @@
 from abc import abstractmethod
 from typing import Union
 
 from onnx import ModelProto, NodeProto, TensorProto
 
 from sparseml.exporters.transforms import BaseTransform
 from sparseml.exporters.transforms.utils import MatchResult
-from sparseml.onnx.utils import ONNXGraph, check_load_model, validate_onnx_file
+from sparseml.onnx.utils import ONNXGraph
+from sparsezoo.utils import load_model, validate_onnx
 
 
 __all__ = ["OnnxTransform"]
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -76,16 +77,16 @@
         :return: The validated ONNX model
         """
         if not ((isinstance(model, str) or isinstance(model, ModelProto))):
             raise ValueError(
                 f"Invalid model type: {type(model)}. "
                 "Must be a string (path to the .onnx file) or ONNX ModelProto"
             )
-        model = check_load_model(model)
-        validate_onnx_file(model)
+        model = load_model(model)
+        validate_onnx(model)
         self._nodes_to_delete.clear()
         self._nodes_to_add.clear()
         self._num_matches = 0
         return model
 
     def post_validate(self, model: ModelProto) -> ModelProto:
         """
@@ -98,9 +99,9 @@
         )
         model.graph.node.extend(self._nodes_to_add)
         for node in self._nodes_to_delete:
             model.graph.node.remove(node)
         graph = ONNXGraph(model)
         graph.delete_unused_initializers()
         graph.sort_nodes_topologically()
-        validate_onnx_file(model)
+        validate_onnx(model)
         return model
```

## sparseml/onnx/optim/analyzer_model.py

```diff
@@ -23,25 +23,25 @@
 import numpy
 from onnx import ModelProto
 
 from sparseml.onnx.optim.sensitivity_pruning import pruning_loss_sens_approx
 from sparseml.onnx.utils import (
     NodeShape,
     calculate_flops,
-    check_load_model,
     extract_node_id,
     extract_node_shapes,
     get_kernel_shape,
     get_node_attributes,
     get_node_inputs,
     get_node_outputs,
     get_node_params,
     is_prunable_node,
 )
 from sparseml.utils import clean_path, create_parent_dirs
+from sparsezoo.utils import load_model
 
 
 __all__ = ["NodeAnalyzer", "ModelAnalyzer"]
 
 
 class NodeAnalyzer(object):
     """
@@ -354,15 +354,15 @@
         if model is None and nodes is None:
             raise ValueError("model or nodes must not be None")
 
         if model is not None and nodes is not None:
             raise ValueError("model or nodes must be None, both cannot be passed")
 
         if model is not None:
-            model = check_load_model(model)
+            model = load_model(model)
             node_shapes = extract_node_shapes(model)
             self._nodes = [
                 NodeAnalyzer(
                     model, node, node_shape=node_shapes.get(extract_node_id(node))
                 )
                 for node in model.graph.node
             ]
```

## sparseml/onnx/optim/sensitivity_pruning.py

```diff
@@ -26,15 +26,14 @@
 from tqdm import auto
 
 from sparseml.onnx.utils import (
     DataLoader,
     DeepSparseAnalyzeModelRunner,
     DeepSparseModelRunner,
     ORTModelRunner,
-    check_load_model,
     extract_node_id,
     get_node_params,
     get_prunable_nodes,
     kl_divergence,
     prune_model_one_shot,
     update_model_param,
 )
@@ -42,14 +41,15 @@
     PruningLossSensitivityAnalysis,
     PruningPerfSensitivityAnalysis,
     PruningSensitivityResult,
     default_pruning_sparsities_loss,
     default_pruning_sparsities_perf,
 )
 from sparseml.utils import flatten_iterable
+from sparsezoo.utils import load_model
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 __all__ = [
     "pruning_loss_sens_approx",
@@ -138,15 +138,15 @@
 
     :param model: the loaded model or a file path to the onnx model
         to calculate the sparse sensitivity analysis for
     :param sparsity_levels: the sparsity levels to calculate the loss for for each param
     :return: the analysis results for the model with an additional layer at each
         iteration along with a float representing the iteration progress
     """
-    model = check_load_model(model)
+    model = load_model(model)
     prunable = get_prunable_nodes(model)
     analysis = PruningLossSensitivityAnalysis()
     num_layers = len(prunable)
 
     for index, node in enumerate(prunable):
         node_id = extract_node_id(node)
 
@@ -247,15 +247,15 @@
         the model for each sparsity level on each node
     :param sparsity_levels: the sparsity levels to calculate the loss for for each param
     :param use_deepsparse_inference: True to use the DeepSparse inference engine
         to run the analysis, False to use onnxruntime
     :return: the sensitivity results for every node that is prunable,
         yields update at each layer along with iteration progress
     """
-    model = check_load_model(model)
+    model = load_model(model)
     prunable_nodes = get_prunable_nodes(model)
     analysis = PruningLossSensitivityAnalysis()
     num_updates = len(prunable_nodes) * len(sparsity_levels) + 1
     update_num = 0
 
     yield analysis, KSSensitivityProgress(update_num, None, num_updates, 0.0)
```

## sparseml/onnx/optim/quantization/calibration.py

```diff
@@ -21,14 +21,15 @@
 import tempfile
 from typing import Dict, Generator, Iterable, List, Tuple, Union
 
 import numpy as np
 import onnx
 
 from sparseml.onnx.utils import ORTModelRunner, fold_conv_bns, get_node_output_nodes
+from sparsezoo.utils import save_onnx, validate_onnx
 
 
 __all__ = ["CalibrationSession"]
 
 
 class CalibrationSession:
     """
@@ -64,15 +65,15 @@
         self._model_augmented = self.generate_augmented_model()
 
         if self._augmented_model_path is None:
             self._augmented_model_tmp_file = tempfile.NamedTemporaryFile(
                 suffix=".onnx", delete=True
             )
             self._augmented_model_path = self._augmented_model_tmp_file.name
-        onnx.save(self._model_augmented, self._augmented_model_path)
+        save_onnx(self._model_augmented, self._augmented_model_path)
 
         self._sessions = {}  # batch_size -> session
         self._quantization_thresholds = {}  # Dict[node.name, Tuple(min_val, max_val)]
 
     @property
     def model(self):
         """
@@ -97,21 +98,19 @@
         """
         try:
             print("Optimizing {}...".format(self._onnx_file))
             model_optimized = fold_conv_bns(self._onnx_file)
             if model_optimized is None:
                 # no optimization performed, skip the rest of this block
                 raise Exception()
-            onnx.checker.check_model(
-                model_optimized
-            )  # should raise exception if broken
+            validate_onnx(model_optimized)  # should raise exception if broken
             optimized_model_path = tempfile.NamedTemporaryFile(
                 suffix=".onnx", delete=False
             )
-            onnx.save(model_optimized, optimized_model_path.name)
+            save_onnx(model_optimized, optimized_model_path.name)
             self._model = model_optimized
             print("Optimization successful")
             return optimized_model_path.name
         except Exception as e:
             print(e)
             print(
                 (
```

## sparseml/onnx/optim/quantization/quantize_model_post_training.py

```diff
@@ -20,14 +20,15 @@
 
 import onnx
 from tqdm.auto import tqdm
 
 from sparseml.onnx.optim.quantization.calibration import CalibrationSession
 from sparseml.onnx.optim.quantization.quantize import QuantizationMode, quantize
 from sparseml.onnx.utils import DataLoader, quantize_resnet_identity_add_inputs
+from sparsezoo.utils import save_onnx
 
 
 __all__ = ["quantize_model_post_training"]
 
 
 def quantize_model_post_training(
     onnx_file: str,
@@ -101,8 +102,8 @@
 
     if run_extra_opt:
         quantize_resnet_identity_add_inputs(calibrated_quantized_model)
 
     if output_model_path is None:
         return calibrated_quantized_model
     else:
-        onnx.save(calibrated_quantized_model, output_model_path)
+        save_onnx(calibrated_quantized_model, output_model_path)
```

## sparseml/onnx/utils/data.py

```diff
@@ -21,21 +21,21 @@
 from collections import OrderedDict
 from typing import Dict, List, Tuple, Union
 
 import numpy
 from onnx import ModelProto
 
 from sparseml.onnx.utils.helpers import (
-    check_load_model,
     extract_shape,
     get_numpy_dtype,
     model_inputs,
     model_outputs,
 )
 from sparseml.utils import NumpyArrayBatcher, load_labeled_data
+from sparsezoo.utils import load_model
 
 
 __all__ = ["DataLoader"]
 
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -167,15 +167,15 @@
             or a positive integer for the desired number of steps
         :param num_samples: number of random samples to create
         :param create_labels: True to create random label data as well, False otherwise
         :param strip_first_dim: True to strip the first dimension from the inputs
             and outputs, typically the batch dimension
         :return: the created DataLoader instance with the random data
         """
-        model = check_load_model(model)
+        model = load_model(model)
         inputs = model_inputs(model)
         outputs = model_outputs(model)
         data_shapes = OrderedDict(
             [
                 (
                     inp.name,
                     extract_shape(inp)[1:] if strip_first_dim else extract_shape(inp),
```

## sparseml/onnx/utils/helpers.py

```diff
@@ -24,22 +24,20 @@
 
 import numpy
 import onnx
 from onnx import ModelProto, NodeProto, TensorProto, numpy_helper
 from onnx.helper import get_attribute_value, make_empty_tensor_value_info
 
 from sparseml.onnx.base import require_onnxruntime
-from sparseml.utils import clean_path
+from sparsezoo.utils import load_model, save_onnx
 
 
 _LOGGER = logging.getLogger(__name__)
 
 __all__ = [
-    "validate_onnx_file",
-    "check_load_model",
     "extract_node_id",
     "get_node_by_id",
     "get_nodes_by_input_id",
     "get_nodes_by_output_id",
     "extract_shape",
     "get_numpy_dtype",
     "NodeShape",
@@ -74,54 +72,14 @@
     "get_tensor_shape",
     "get_tensor_dim_shape",
     "set_tensor_dim_shape",
     "override_model_input_shape",
 ]
 
 
-def validate_onnx_file(path: str):
-    """
-    Validate that a file at a given path is a valid ONNX model
-
-    :param path: the path of the file to validate
-    :raise ValueError: if not a valid ONNX model
-    """
-    try:
-        onnx_model = check_load_model(path)
-
-        if onnx_model.ByteSize() < onnx.checker.MAXIMUM_PROTOBUF:
-            onnx.checker.check_model(onnx_model)
-        else:
-            _LOGGER.warning(
-                "onnx check_model skipped as model exceeds maximum protobuf size of 2GB"
-            )
-
-        if not onnx_model.opset_import:
-            raise ValueError("could not parse opset_import")
-    except Exception as err:
-        raise ValueError(f"Invalid onnx model: {err}")
-
-
-def check_load_model(model: Union[str, ModelProto]) -> ModelProto:
-    """
-    Load an ONNX model from a given file path if supplied.
-    If already a model proto, then returns.
-
-    :param model: the model proto or path to the model ONNX file to check for loading
-    :return: the loaded ONNX ModelProto
-    """
-    if isinstance(model, ModelProto):
-        return model
-
-    if isinstance(model, str):
-        return onnx.load(clean_path(model))
-
-    raise ValueError(f"unknown type given for model: {type(model)}")
-
-
 def extract_node_id(node: NodeProto) -> str:
     """
     Get the node id for a given node from an ONNX model.
     Grabs the first ouput id as the node id.
     This is because is guaranteed to be unique for this node by the ONNX spec.
 
     :param node: the node to grab an id for
@@ -911,15 +869,15 @@
     """
     Get the prunable nodes in an ONNX model proto.
     Prunable nodes are defined as any conv, gemm, or matmul
 
     :param model: the model proto loaded from the ONNX file
     :return: a list of nodes from the model proto
     """
-    model = check_load_model(model)
+    model = load_model(model)
     prunable_nodes = []
 
     for node in model.graph.node:
         if is_prunable_node(model, node):
             prunable_nodes.append(node)
 
     return prunable_nodes
@@ -947,15 +905,15 @@
     Retrieve the sparsities for each Conv or Gemm op in an ONNX graph
     for the associated weight inputs.
 
     :param model: ONNX model to use
     :return: a tuple containing the overall sparsity measurement for the model,
         each conv or gemm node found in the model
     """
-    model = check_load_model(model)
+    model = load_model(model)
     node_inp_sparsities = OrderedDict()  # type: Dict[str, SparsityMeasurement]
     params_count = 0
     params_zero_count = 0
 
     for node in get_prunable_nodes(model):
         node_id = extract_node_id(node)
         node_key = "{}(id={})".format(node.op_type, node_id)
@@ -987,15 +945,15 @@
     """
     Get the input to the model from an ONNX model
 
     :param model: the loaded model or a file path to the ONNX model
         to get the model inputs for
     :return: the input to the model
     """
-    model = check_load_model(model)
+    model = load_model(model)
     inputs_all = [node.name for node in model.graph.input]
     inputs_init = [node.name for node in model.graph.initializer]
     input_names = list(set(inputs_all) - set(inputs_init))
     inputs = [node for node in model.graph.input if node.name in input_names]
     assert len(input_names) == len(inputs)
 
     return inputs
@@ -1005,15 +963,15 @@
     """
     Get the output from an ONNX model
 
     :param model: the loaded model or a file path to the ONNX model
         to get the model outputs for
     :return: the output from the model
     """
-    model = check_load_model(model)
+    model = load_model(model)
     outputs = [node for node in model.graph.output]
 
     return outputs
 
 
 def get_kernel_shape(attributes: Dict[str, Any]) -> Union[List[float], None]:
     """
@@ -1268,8 +1226,8 @@
     else:
         model_path = None
 
     for dim, dim_size in enumerate(shape):
         set_tensor_dim_shape(model.graph.input[0], dim, dim_size)
 
     if model_path:
-        onnx.save(model, model_path)
+        save_onnx(model, model_path)
```

## sparseml/onnx/utils/model.py

```diff
@@ -30,21 +30,21 @@
 from onnx import ModelProto
 from tqdm import auto
 
 from sparseml.onnx.base import require_onnxruntime
 from sparseml.onnx.utils.data import DataLoader
 from sparseml.onnx.utils.graph_editor import override_model_batch_size
 from sparseml.onnx.utils.helpers import (
-    check_load_model,
     extract_node_id,
     get_node_by_id,
     get_prunable_node_from_foldable,
     is_foldable_node,
 )
 from sparsezoo import File, Model
+from sparsezoo.utils import load_model
 
 
 try:
     import deepsparse
     from deepsparse import compile_model, model_debug_analysis
     from deepsparse.cpu import cpu_details
 except Exception:
@@ -460,15 +460,15 @@
         batch_size: int = None,
         providers: List[str] = None,
         **kwargs,
     ):
         import onnxruntime  # import protected by @require_onnxruntime()
 
         super().__init__(loss)
-        self._model = check_load_model(model)
+        self._model = load_model(model)
 
         if batch_size is not None:
             override_model_batch_size(self._model, batch_size)
         # default selected providers to ort default
         providers = providers or onnxruntime.get_available_providers()
 
         sess_options = onnxruntime.SessionOptions()
@@ -708,15 +708,15 @@
     Additionally, ops that did not have an id are changed from the returned
     string <none> to proper None python type
 
     :param nm_result: the result from the deepsparse.analyze_model api
     :param model: the onnx model proto or path to the onnx file that the
         nm_result was for
     """
-    model = check_load_model(model)
+    model = load_model(model)
 
     for layer in nm_result["layer_info"]:
         node_id = (
             layer["canonical_name"] if "<none>" not in layer["canonical_name"] else None
         )
 
         if node_id is None:
```

## sparseml/openpifpaf/export.py

```diff
@@ -15,20 +15,20 @@
 # limitations under the License.
 
 import argparse
 import logging
 import os
 from typing import Optional
 
-import onnx
 import torch
 
 import openpifpaf
 from sparseml.pytorch.optim.manager import ScheduledModifierManager
 from sparseml.pytorch.utils import ModuleExporter
+from sparsezoo.utils import validate_onnx
 
 
 LOG = logging.getLogger(__name__)
 
 
 def image_size_warning(basenet_stride, input_w, input_h):
     if input_w % basenet_stride != 1:
@@ -111,13 +111,13 @@
     exporter = ModuleExporter(model, save_dir)
     exporter.export_onnx(
         torch.randn(1, 3, input_height, input_width),
         name=name,
         input_names=["input_batch"],
         output_names=[meta.name for meta in datamodule.head_metas],
     )
-    onnx.checker.check_model(os.path.join(save_dir, name))
+    validate_onnx(os.path.join(save_dir, name))
     exporter.create_deployment_folder()
 
 
 if __name__ == "__main__":
     main()
```

## sparseml/pytorch/torch_to_onnx_exporter.py

```diff
@@ -26,14 +26,15 @@
 from sparseml.exporters import transforms as sparseml_transforms
 from sparseml.exporters.base_exporter import BaseExporter
 from sparseml.exporters.transforms.base_transform import BaseTransform
 from sparseml.pytorch import _PARSED_TORCH_VERSION
 from sparseml.pytorch.opset import TORCH_DEFAULT_ONNX_OPSET
 from sparseml.pytorch.utils.helpers import tensors_module_forward, tensors_to_device
 from sparseml.pytorch.utils.model import is_parallel_model
+from sparsezoo.utils import save_onnx
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class TorchToONNX(BaseExporter):
     """
@@ -97,15 +98,15 @@
     def post_validate(self, model: onnx.ModelProto) -> onnx.ModelProto:
         if not isinstance(model, onnx.ModelProto):
             raise TypeError(f"Expected onnx.ModelProto, found {type(model)}")
         return model
 
     def export(self, pre_transforms_model: torch.nn.Module, file_path: str):
         post_transforms_model: onnx.ModelProto = self.apply(pre_transforms_model)
-        onnx.save(post_transforms_model, file_path)
+        save_onnx(post_transforms_model, file_path)
 
 
 class _TorchOnnxExport(BaseTransform):
     def __init__(
         self,
         sample_batch: Any,
         opset: int = TORCH_DEFAULT_ONNX_OPSET,
```

## sparseml/pytorch/sparsification/quantization/quantize_qat_export.py

```diff
@@ -35,14 +35,15 @@
     get_node_attributes,
     get_node_output_nodes,
     quantize_resnet_identity_add_inputs,
     remove_node_and_params_from_graph,
     swap_node_output,
     update_model_param,
 )
+from sparsezoo.utils import save_onnx
 
 
 __all__ = [
     "get_quantization_params",
     "QuantizationParams",
     "quantize_torch_qat_export",
     "skip_onnx_input_quantize",
@@ -1589,15 +1590,15 @@
     _convert_signed_to_unsigned(model)
 
     graph = ONNXGraph(model)
     graph.sort_nodes_topologically()
     graph.delete_unused_initializers()
 
     if output_file_path:
-        onnx.save(model, output_file_path)
+        save_onnx(model, output_file_path)
 
     return model
 
 
 def _delete_quantize_nodes(graph: ONNXGraph, quantize_nodes: List[NodeProto]):
     # delete given quantize nodes and forward their inputs to the next graph layer
     for quantize_node in quantize_nodes:
@@ -1714,15 +1715,15 @@
 
     optim_error_message = _skip_input_quantize(model)
 
     if optim_error_message and not _skip_trivially_nested_input_quantize(model):
         raise RuntimeError(optim_error_message)
 
     if output_file_path:
-        onnx.save(model, output_file_path)
+        save_onnx(model, output_file_path)
 
 
 def _propagate_mobilebert_embedding_quantization(model: ModelProto):
     """
     A pass for propagating embedding quantizations through concat
 
     Starting with:
```

## sparseml/pytorch/utils/exporter.py

```diff
@@ -44,14 +44,15 @@
 from sparseml.pytorch.utils.model import (
     is_parallel_model,
     save_model,
     script_model,
     trace_model,
 )
 from sparseml.utils import clean_path, create_parent_dirs
+from sparsezoo.utils import save_onnx, validate_onnx
 
 
 __all__ = [
     "ModuleExporter",
     "export_onnx",
 ]
 
@@ -566,15 +567,15 @@
     _flatten_qparams(onnx_model)
     if batch_norms_wrapped:
         # fix changed batch norm names
         _unwrap_batchnorms(onnx_model)
 
         # clean up graph from any injected / wrapped operations
         _delete_trivial_onnx_adds(onnx_model)
-    onnx.save(onnx_model, file_path)
+    save_onnx(onnx_model, file_path)
 
     if convert_qat and is_quant_module:
         # overwrite exported model with fully quantized version
         # import here to avoid cyclic dependency
         from sparseml.pytorch.sparsification.quantization import (
             quantize_torch_qat_export,
         )
@@ -815,8 +816,8 @@
         init.name = init.name.replace(".bn_wrapper_replace_me", "")
     for node in model.graph.node:
         for idx in range(len(node.input)):
             node.input[idx] = node.input[idx].replace(".bn_wrapper_replace_me", "")
         for idx in range(len(node.output)):
             node.output[idx] = node.output[idx].replace(".bn_wrapper_replace_me", "")
 
-    onnx.checker.check_model(model)
+    validate_onnx(model)
```

## sparseml/transformers/export.py

```diff
@@ -87,20 +87,21 @@
 from sparseml.transformers.sparsification import Trainer
 from sparseml.transformers.utils import SparseAutoModel
 
 
 __all__ = ["export_transformer_to_onnx", "load_task_model"]
 
 MODEL_ONNX_NAME = "model.onnx"
-DEPLOYMENT_FILES: List[str] = [
+EXTERNAL_ONNX_DATA_NAME = "model.data"
+MANDATORY_DEPLOYMENT_FILES: List[str] = [
     MODEL_ONNX_NAME,
-    "tokenizer.json",
     "tokenizer_config.json",
     "config.json",
 ]
+OPTIONAL_DEPLOYMENT_FILES: List[str] = [EXTERNAL_ONNX_DATA_NAME, "tokenizer.json"]
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def load_task_model(task: str, model_path: str, config: Any) -> Module:
     if task == "masked-language-modeling" or task == "mlm":
         return SparseAutoModel.masked_language_modeling_from_pretrained(
@@ -399,37 +400,48 @@
     :param deployment_files: optional list of deployment file names to override
         default file names with.
     :return: path to the valid deployment directory
     """
 
     if deployment_files is None:
         # set deployment files to default values
-        deployment_files = copy.deepcopy(DEPLOYMENT_FILES)
+        deployment_files = copy.deepcopy(
+            MANDATORY_DEPLOYMENT_FILES + OPTIONAL_DEPLOYMENT_FILES
+        )
         if onnx_file_name != MODEL_ONNX_NAME:
             # replace the default onnx model name with the custom one
             deployment_files[deployment_files.index(MODEL_ONNX_NAME)] = onnx_file_name
 
     model_root_dir = os.path.dirname(training_directory)
     deployment_folder_dir = os.path.join(model_root_dir, "deployment")
     if os.path.isdir(deployment_folder_dir):
         shutil.rmtree(deployment_folder_dir)
     os.makedirs(deployment_folder_dir)
 
     for file_name in deployment_files:
         expected_file_path = os.path.join(training_directory, file_name)
         deployment_file_path = os.path.join(deployment_folder_dir, file_name)
         if not os.path.exists(expected_file_path):
+            if file_name in OPTIONAL_DEPLOYMENT_FILES:
+                _LOGGER.warning(
+                    f"Optional file {file_name} not found in {training_directory}. "
+                    f"Skipping copying to deployment folder."
+                )
+                continue
             raise ValueError(
                 f"Attempting to copy {file_name} file from {expected_file_path},"
                 f"but the file does not exits. Make sure that {training_directory} "
                 f"contains following files: {deployment_files}"
             )
         if file_name == MODEL_ONNX_NAME:
             # moving onnx file from training to deployment directory
             shutil.move(expected_file_path, deployment_file_path)
+        elif file_name == EXTERNAL_ONNX_DATA_NAME:
+            # moving external onnx tensors from training to deployment directory
+            shutil.move(expected_file_path, deployment_file_path)
         else:
             # copying remaining `deployment_files` from training to deployment directory
             shutil.copyfile(expected_file_path, deployment_file_path)
         _LOGGER.info(
             f"Saved {file_name} in the deployment folder at {deployment_file_path}"
         )
     return deployment_folder_dir
```

## sparseml/transformers/masked_language_modeling.py

```diff
@@ -47,33 +47,28 @@
     AutoConfig,
     AutoTokenizer,
     DataCollatorForLanguageModeling,
     HfArgumentParser,
     set_seed,
 )
 from transformers.trainer_utils import get_last_checkpoint
-from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
 
 from sparseml.pytorch.utils.distributed import record
 from sparseml.transformers.sparsification import Trainer, TrainingArguments
 from sparseml.transformers.utils import SparseAutoModel, get_shared_tokenizer_src
 
 
 metadata_args = [
     "per_device_train_batch_size",
     "per_device_eval_batch_size",
     "fp16",
 ]
 
 
-# Will error if the minimal version of Transformers is not installed.
-# Remove at your own risks
-check_min_version("4.18.0.dev0")
-
 require_version(
     "datasets>=1.18.0",
     "To fix: pip install -r examples/pytorch/language-modeling/requirements.txt",
 )
 
 _LOGGER = logging.getLogger(__name__)
 MODEL_CONFIG_CLASSES = list(MODEL_FOR_MASKED_LM_MAPPING.keys())
```

## sparseml/transformers/question_answering.py

```diff
@@ -41,30 +41,25 @@
     EvalPrediction,
     HfArgumentParser,
     PreTrainedTokenizerFast,
     default_data_collator,
     set_seed,
 )
 from transformers.trainer_utils import get_last_checkpoint
-from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
 
 from sparseml.pytorch.utils.distributed import record
 from sparseml.transformers.sparsification import (
     QuestionAnsweringTrainer,
     TrainingArguments,
     postprocess_qa_predictions,
 )
 from sparseml.transformers.utils import SparseAutoModel, get_shared_tokenizer_src
 
 
-# Will error if the minimal version of Transformers is not installed. Remove at your
-# own risks.
-check_min_version("4.18.0.dev0")
-
 require_version(
     "datasets>=1.18.0",
     "To fix: pip install -r examples/pytorch/question-answering/requirements.txt",
 )
 
 
 _LOGGER = logging.getLogger(__name__)
```

## sparseml/transformers/text_classification.py

```diff
@@ -45,30 +45,25 @@
     EvalPrediction,
     HfArgumentParser,
     PretrainedConfig,
     default_data_collator,
     set_seed,
 )
 from transformers.trainer_utils import get_last_checkpoint
-from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
 
 from sparseml.pytorch.utils.distributed import record
 from sparseml.transformers.sparsification import Trainer, TrainingArguments
 from sparseml.transformers.utils import (
     SparseAutoModel,
     get_shared_tokenizer_src,
     multi_label_precision_recall_f1,
 )
 
 
-# Will error if the minimal version of Transformers is not installed.
-# Remove at your own risks.
-check_min_version("4.18.0.dev0")
-
 require_version(
     "datasets>=1.18.0",
     "To fix: pip install -r examples/pytorch/text-classification/requirements.txt",
 )
 
 _TASK_TO_KEYS = {
     "cola": ("sentence", None),
```

## sparseml/transformers/token_classification.py

```diff
@@ -44,26 +44,21 @@
     DataCollatorForTokenClassification,
     HfArgumentParser,
     PretrainedConfig,
     PreTrainedTokenizerFast,
     set_seed,
 )
 from transformers.trainer_utils import get_last_checkpoint
-from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
 
 from sparseml.pytorch.utils.distributed import record
 from sparseml.transformers.sparsification import Trainer, TrainingArguments
 from sparseml.transformers.utils import SparseAutoModel, get_shared_tokenizer_src
 
 
-# Will error if the minimal version of Transformers is not installed.
-# Remove at your own risks
-check_min_version("4.18.0.dev0")
-
 require_version(
     "datasets>=1.18.0",
     "To fix: pip install -r examples/pytorch/token-classification/requirements.txt",
 )
 
 _LOGGER: logging.Logger = logging.getLogger(__name__)
```

## sparseml/yolov8/trainers.py

```diff
@@ -19,15 +19,14 @@
 import tempfile
 import warnings
 from copy import copy, deepcopy
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import List, Optional
 
-import onnx
 import torch
 
 from sparseml.optim.helpers import load_recipe_yaml_str
 from sparseml.pytorch.optim.manager import ScheduledModifierManager
 from sparseml.pytorch.sparsification.quantization import skip_onnx_input_quantize
 from sparseml.pytorch.utils import ModuleExporter
 from sparseml.pytorch.utils.helpers import download_framework_model_by_recipe_type
@@ -41,14 +40,15 @@
 from sparseml.yolov8.utils.export_samples import export_sample_inputs_outputs
 from sparseml.yolov8.validators import (
     SparseClassificationValidator,
     SparseDetectionValidator,
     SparseSegmentationValidator,
 )
 from sparsezoo import Model
+from sparsezoo.utils import validate_onnx
 from ultralytics import __version__
 from ultralytics.nn.tasks import SegmentationModel, attempt_load_one_weight
 from ultralytics.yolo.cfg import get_cfg
 from ultralytics.yolo.data.dataloaders.v5loader import create_dataloader
 from ultralytics.yolo.engine.model import YOLO
 from ultralytics.yolo.engine.trainer import BaseTrainer
 from ultralytics.yolo.utils import LOGGER, IterableSimpleNamespace, yaml_load
@@ -724,15 +724,15 @@
 
         complete_path = os.path.join(save_dir, name)
         try:
             skip_onnx_input_quantize(complete_path, complete_path)
         except Exception:
             pass
 
-        onnx.checker.check_model(complete_path)
+        validate_onnx(complete_path)
         deployment_folder = exporter.create_deployment_folder(onnx_model_name=name)
         if args["export_samples"]:
             trainer_config = get_cfg(cfg=DEFAULT_SPARSEML_CONFIG_PATH)
 
             if args["dataset_path"] is not None:
                 args["data"] = data_from_dataset_path(
                     args["data"], args["dataset_path"]
```

## Comparing `sparseml_nightly-1.5.0.20230509.dist-info/LICENSE` & `sparseml_nightly-1.5.0.20230516.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230509.dist-info/METADATA` & `sparseml_nightly-1.5.0.20230516.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.5.0.20230509
+Version: 1.5.0.20230516
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -89,33 +89,33 @@
 Requires-Dist: tf2onnx (<1.6,>=1.0.0) ; extra == 'tf_v1_gpu'
 Provides-Extra: torch
 Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'torch'
 Requires-Dist: gputils ; extra == 'torch'
 Provides-Extra: torch_all
 Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'torch_all'
 Requires-Dist: gputils ; extra == 'torch_all'
-Requires-Dist: torchvision (<=0.14,>=0.3.0) ; extra == 'torch_all'
+Requires-Dist: torchvision (<0.15,>=0.3.0) ; extra == 'torch_all'
 Requires-Dist: torchaudio (<=0.13) ; extra == 'torch_all'
 Provides-Extra: torchvision
 Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'torchvision'
 Requires-Dist: gputils ; extra == 'torchvision'
-Requires-Dist: torchvision (<=0.14,>=0.3.0) ; extra == 'torchvision'
+Requires-Dist: torchvision (<0.15,>=0.3.0) ; extra == 'torchvision'
 Provides-Extra: transformers
 Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'transformers'
 Requires-Dist: gputils ; extra == 'transformers'
 Requires-Dist: nm-transformers-nightly (~=1.5.0) ; extra == 'transformers'
 Requires-Dist: datasets (<=1.18.4) ; extra == 'transformers'
 Requires-Dist: scikit-learn ; extra == 'transformers'
 Requires-Dist: seqeval ; extra == 'transformers'
 Provides-Extra: ultralytics
 Requires-Dist: ultralytics (==8.0.30) ; extra == 'ultralytics'
 Provides-Extra: yolov5
 Requires-Dist: torch (<=1.13.1,>=1.1.0) ; extra == 'yolov5'
 Requires-Dist: gputils ; extra == 'yolov5'
-Requires-Dist: torchvision (<=0.14,>=0.3.0) ; extra == 'yolov5'
+Requires-Dist: torchvision (<0.15,>=0.3.0) ; extra == 'yolov5'
 Requires-Dist: nm-yolov5-nightly (~=1.5.0) ; extra == 'yolov5'
 
 <!--
 Copyright (c) 2021 - present / Neuralmagic, Inc. All Rights Reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
```

## Comparing `sparseml_nightly-1.5.0.20230509.dist-info/NOTICE` & `sparseml_nightly-1.5.0.20230516.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230509.dist-info/entry_points.txt` & `sparseml_nightly-1.5.0.20230516.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.5.0.20230509.dist-info/RECORD` & `sparseml_nightly-1.5.0.20230516.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 sparseml/deepsparse/base.py,sha256=nRjU6TSao0J2iWXcdHwj62X6dVT9vl6TQ2y4Bdn3KN0,3516
 sparseml/deepsparse/framework/__init__.py,sha256=ZHrXXM3AMH78zKcF8Y40IBuy38UFy4fLrvytozw_bNY,801
 sparseml/deepsparse/framework/info.py,sha256=HVDPHFXggFeDqbpM20PkByf1nBccwKnjpTWh0EfrVas,6032
 sparseml/deepsparse/sparsification/__init__.py,sha256=re_2FtHWvO-iQQwRRJZDKz3l_pFZuwe266-4ZFxQqbY,813
 sparseml/deepsparse/sparsification/info.py,sha256=O5FJg5KMJvj-HcJn9W9iiKGZ6Z7_1SavOX-TstXRr6Q,1348
 sparseml/exporters/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
 sparseml/exporters/base_exporter.py,sha256=M1HEe9GNf51uYx1z-qxWjIYo5iGZ_Ish8uZ3mj6OZR8,1477
-sparseml/exporters/onnx_to_deepsparse.py,sha256=X2yFfvJomwLOGHfe_ZmmosPc0Pa4Bjmw81q0uv_Rq18,4751
+sparseml/exporters/onnx_to_deepsparse.py,sha256=OO7WosKj8jtd-pSoh7RzaJh-ScWPHV7d-F75gOvJu08,4783
 sparseml/exporters/transforms/__init__.py,sha256=bitsfVa9RUFuZYVUD4oxEh_IqEyiQQuxIYaGA8rOt2w,2252
 sparseml/exporters/transforms/base_transform.py,sha256=IpvdUdEADl2SfqHawcp6-lcNgz-R3L0zpS05WaWF5h8,2333
 sparseml/exporters/transforms/constants_to_initializers.py,sha256=_PX3y16OC-q85d-6DeOOVpKAAMNIU1m5BdYTZlFV_tk,1388
 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py,sha256=9z2HRqJAM68HPiSfu2RMyrn93dr8HCTpMcMrh_1-x2w,3866
 sparseml/exporters/transforms/conv_to_qlinearconv.py,sha256=CwCXtIBCOQ1qX5Z2JZhsdXSDk683wRCIBILF_1vd0GI,5838
 sparseml/exporters/transforms/delete_repeated_qdq.py,sha256=YiIOrvKqrxYboOA4A8YTbQIQ4s4MDdmqeLNYHPP4kjs,2440
 sparseml/exporters/transforms/delete_trivial_onnx_adds.py,sha256=St3-PQP8tPXYoyQTFn8fvJi7JF3LoX9Vb9nc-Zbx4Wg,1842
@@ -28,15 +28,15 @@
 sparseml/exporters/transforms/fold_relu_quants.py,sha256=qDGl-6aGmaQ8lAii3v0NvqkjbqtZB1UgHEkd3RzvjXQ,2070
 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py,sha256=r1oVnnu-U0mISkqBJrebXO1o-cmbkSMbo1X4xA0l-t4,4418
 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py,sha256=ccrB80ymufz6c9znwIGz0rxvM6U-vmKqiCa7l0vKYfE,7629
 sparseml/exporters/transforms/initializers_to_uint8.py,sha256=GxveAKe1xSNBZh1hjUx61veL6LTf9Msnx663Mrhvtxg,1645
 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py,sha256=1YxX2xm2JC3IUj4AuRxRf2yXeOWj-esLLo-aoL_LtOo,4470
 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py,sha256=l3JXoue_8Rs8DMGaH_MCNBR5RZRIzIhXiM5D_TRS81M,4571
 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py,sha256=Siii4mZ3LtqWY1blD1KT7ePVJud1oyLDrcr21YosU7E,4156
-sparseml/exporters/transforms/onnx_transform.py,sha256=o3jRAOag020HzYRtqQdp-CXEFReZm3yGng7tHvqWM5Q,3724
+sparseml/exporters/transforms/onnx_transform.py,sha256=vqlJJTjqZx9IUV3woHjKnWQMl2w-iurZK2eGABhYX9M,3724
 sparseml/exporters/transforms/propagate_embedding_quantization.py,sha256=XTEiUTX5nzLUtndGs_0t7nTgjIad-FyjuNc0O4f6Xro,3398
 sparseml/exporters/transforms/quantize_qat_embedding.py,sha256=_v1dEEt5vCSaMF6dJkg9fVGof145-_Lmo0DMjpXsnUE,4464
 sparseml/exporters/transforms/quantize_residuals.py,sha256=f3kNF930ymHI5CmCA0OmYW7vDKvEm9sYhN0UX0UC1EQ,3869
 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py,sha256=mod-7bnlkg20LjerZ7tKKmp_7XyO3FKo13BtIZkDsmM,3331
 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py,sha256=2FSXzaY3jdxOgj3xBaUOUqtk-hzg4kwhheELhoOKpS8,2545
 sparseml/exporters/transforms/skip_input_quantize.py,sha256=ANiYDwSos9gPW4960fMwmGubTDgpAcqFVSIHKf_ffYw,3210
 sparseml/exporters/transforms/unwrap_batchnorms.py,sha256=ly7GHCXN_2r8Gnk8PABWCqcoS-NL3GMfquEK0hRlFCs,1373
@@ -85,47 +85,47 @@
 sparseml/onnx/__init__.py,sha256=KeWF6EQ7cpX_b-fMhiG5n6pVPUvRxiWMpzpiI9EagFI,1036
 sparseml/onnx/base.py,sha256=Kv3YC0Xh1xlxpIuwh9916SHuz96phaf36KbL71DSZWk,6202
 sparseml/onnx/benchmark/__init__.py,sha256=tl8cy1ta02lUmMxwmDfRAYcVQfaj5OpU3igqYJHMGg8,743
 sparseml/onnx/benchmark/info.py,sha256=iCNry2VAuSmTLrPl3a8pxDU_R-U9-Lpcka40QIg5BZg,15366
 sparseml/onnx/framework/__init__.py,sha256=HpgplVizgXIPOmnE24RM1geQLp924227_T12jJjQCaA,823
 sparseml/onnx/framework/info.py,sha256=YzZmDaR6Z1y66xo_OKtmQGA1ZVFOozZNXBJ_Ec74ueU,6116
 sparseml/onnx/optim/__init__.py,sha256=EZeHGH5zDRfb0MrXqh4_3ci0ViBS2WWb8NqhAi8nd3A,820
-sparseml/onnx/optim/analyzer_model.py,sha256=NLxYEH9QaU-xl2h1SagMHyfQ3skEsuYRFTqeYpKTgIM,13274
-sparseml/onnx/optim/sensitivity_pruning.py,sha256=uibp_XyIwFID8J-Gym-00R0WQgw0Zai7ByDUyhnLlEE,19634
+sparseml/onnx/optim/analyzer_model.py,sha256=6nfKmLzdwesxupN_PWNLCGtXPk2uf4L5OOBBuzSNvQ4,13285
+sparseml/onnx/optim/sensitivity_pruning.py,sha256=L-Sp669RNH4BaZJ3JTcDvcoaOZEE1URFxALPVq3z9rY,19639
 sparseml/onnx/optim/structured_pruning.py,sha256=XyyoNqa7855JM-R3B6UgSez2h4V1EuEi4jUhuK0ztT8,6470
 sparseml/onnx/optim/quantization/__init__.py,sha256=mKe75Yza1RlQOe43pcLb-IzWJD34LhwAALF7LYU2f2E,815
-sparseml/onnx/optim/quantization/calibration.py,sha256=LGguzFAMfqu57lBSfus79hMFuq7YduWW7HRn6svXjvs,14520
+sparseml/onnx/optim/quantization/calibration.py,sha256=cVcUyv4aXiTBeUMM7PSl7Ta7OJICVS63WJB2jBqWJFM,14532
 sparseml/onnx/optim/quantization/quantize.py,sha256=TXrlfpE3NssIJuAzdDctWG3w9jCF82PXJDC46GRMJLA,73551
-sparseml/onnx/optim/quantization/quantize_model_post_training.py,sha256=EAcb7Tp8NKX8BZ4FWzzypfWgN09mcQ9zLaVWX66Thgw,4514
+sparseml/onnx/optim/quantization/quantize_model_post_training.py,sha256=aoz5ixUpQB_6XkowhozqRp8_njthBeqVuwvV2ctM1q0,4552
 sparseml/onnx/sparsification/__init__.py,sha256=hFZDQQXFcXqSqiXlRBRUX7e7GavLphgRd8c21peq8fg,869
 sparseml/onnx/sparsification/analyzer.py,sha256=DCKc8nYo0i3NDu73GVjvBYjuflXUZhkhB14FoFRlTBE,10209
 sparseml/onnx/sparsification/info.py,sha256=UnrwVgOuj-HErwTMc-19h-QOrs1yG_mM45O9VL8oiXU,1363
 sparseml/onnx/sparsification/model_info.py,sha256=Y0tpY9fWN3gr4KlkAdXv2QYJrrrjMvVZOCA-ujPJFPM,8009
 sparseml/onnx/utils/__init__.py,sha256=fGZED95Xmko70ZmTWlZWX3-C4dajmbZcKgaap3HXmVw,867
-sparseml/onnx/utils/data.py,sha256=6Rw3hkSG1DZ057USkzioSDFcYH92ZLwdHYlQY2PdkwQ,13002
+sparseml/onnx/utils/data.py,sha256=eh1URN6lmPpVUTg_iHK1R6lLKi4jJh3XGg5OPkgGD_Y,13013
 sparseml/onnx/utils/graph_editor.py,sha256=IBNbKWjOLy7oW-bjsxBkSw5HULHIoeVFQFs2ccYVTs0,16407
 sparseml/onnx/utils/graph_optimizer.py,sha256=AfS2zdxW1tJ6xYAe-2n3KdAdDenxiqslOFUIVAzD-cY,8133
-sparseml/onnx/utils/helpers.py,sha256=zgwIicGlSfVXATOdtpcZbcq3cW8IK0IaOCv_9TR4Ol8,41529
+sparseml/onnx/utils/helpers.py,sha256=I1CJ8loycHBNR35ZaBKxnoFA9TwPHwTEjKlsH1jIgQc,40230
 sparseml/onnx/utils/loss.py,sha256=2njnY0qY2n6DS9HHB0kqLz7N8wgPaDTkAi6Z2DLYPLc,1958
-sparseml/onnx/utils/model.py,sha256=ElcSfKhUnqvjpYusg4iD-pL-y77T14mvECDBPPGnNnQ,31586
+sparseml/onnx/utils/model.py,sha256=jpuomHDXg4pMngluDRGvGPTO1qhTmyRLTMoHasAC8Co,31591
 sparseml/onnx/utils/sparse_tensor.py,sha256=6Bu9fVJqLCtve3qpg9ScYGqcv4X7ZcRKhVrp8pCLBRI,5437
 sparseml/openpifpaf/__init__.py,sha256=cRAMNGqBJbWxG6ds0WRxQnTnvtm_DJqaSBwEt0HupT0,734
-sparseml/openpifpaf/export.py,sha256=YkX06A384K17AfKYli1RcYHcoVg4gF79ttZ-73H_6rI,3694
+sparseml/openpifpaf/export.py,sha256=XkAKuXcCJ64RPZ1YwqzyJKfr9pnn3b0GcROKRXnAWeg,3713
 sparseml/openpifpaf/train.py,sha256=vl5ioCcnzep9XNVMOsveO9QRRrXSn8VDnEM1LGv71Ew,10950
 sparseml/openpifpaf/trainer.py,sha256=Du9W5fW9ImC3XlOVVWesbcBv1SjJOfP_D94_hBUR6VY,4211
 sparseml/optim/__init__.py,sha256=3oGQ4LY0MSrbTAwuyPHEOEyYiZ7JI7OX2BgWup5NPuw,882
 sparseml/optim/analyzer.py,sha256=LUYBYyvfVwaw_V1aAiOmaybUGJQk4vRK5RG3k3nD7pA,6302
 sparseml/optim/helpers.py,sha256=Zb7YPYe07vuVyYUhHJ-BlcMrZa-sxt1TUZ-Ec9Z6o_U,25563
 sparseml/optim/manager.py,sha256=KeDVHj9ea9EUaV908qfvq8ONwS8nUmAvQb1yXflOBWo,25984
 sparseml/optim/modifier.py,sha256=qYfVUL9thw94p4oEsNZgitUJ3y9izWYb8nUI3enyzOU,30708
 sparseml/optim/sensitivity.py,sha256=neMP_hTRqzDUV0MrATevC2-JQYnOIvNW_AlIf_y_ydw,26315
 sparseml/pytorch/__init__.py,sha256=3E40C1X1fjhlU0ZwdHZ-xhORHb-qDUtr7ALDv9xbzI0,1848
 sparseml/pytorch/base.py,sha256=-RvI-RM0ZynTCrsX0VaN_aoDPUdfCc1E1MeUY1VWFH8,6173
 sparseml/pytorch/opset.py,sha256=-BsKarkkKfq09HYJLZfxt_AEHEfuENpRDZF_J2va1Ck,933
-sparseml/pytorch/torch_to_onnx_exporter.py,sha256=hluxRT9RdpIeZmA4Z4KU-ajielvT_09rov-1MYDCR08,10826
+sparseml/pytorch/torch_to_onnx_exporter.py,sha256=78Ft0yuGVKx3TMhPeG9e3o6dI2GC_432VwuiKokfZuc,10864
 sparseml/pytorch/datasets/__init__.py,sha256=2xoH_fCMojldFY1RCWSkt9pGfa8SzHAxU5em-_ZiwV8,998
 sparseml/pytorch/datasets/generic.py,sha256=nl-fFlpd7u5sNswe1AORZvQUne3sqrrPWnNgOUp6_Fc,4193
 sparseml/pytorch/datasets/registry.py,sha256=cEA3d5ju5EMft92f2StVLWARnAxlRpidKZaozujmFdE,2814
 sparseml/pytorch/datasets/classification/__init__.py,sha256=GMKhziJkRwSC7E_1Nox8FxnxhPFozZ6MxQWUWi1BN_Y,828
 sparseml/pytorch/datasets/classification/cifar.py,sha256=k32Z552YrrJv7IlshH8AWylaRKCOUC8KSrzRLLTHTag,4017
 sparseml/pytorch/datasets/classification/imagefolder.py,sha256=rOvwqy2Zp89VkT7zat2hQxRmgPyvCpSAhZ4mWEsL9JI,3669
 sparseml/pytorch/datasets/classification/imagenet.py,sha256=CHzsckzsSsUCLR-oxaxJ8NH7j4WBqg_Wg5ge27bPk5Q,4000
@@ -217,15 +217,15 @@
 sparseml/pytorch/sparsification/quantization/__init__.py,sha256=OjbeCzzhoeFJEJQvLmXZc89pghO83sLRhmvNF7_q_oQ,813
 sparseml/pytorch/sparsification/quantization/constants.py,sha256=sla-j0QwLFq92AbDZkHkNLxugpGrNEQJIuLWoWqV3Ks,2220
 sparseml/pytorch/sparsification/quantization/helpers.py,sha256=MmY5iOMlBUBEMrotPyj3H5drzpXhf13v4FJjb1N2aaw,32271
 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py,sha256=TToI4dGYZZEzB1q61m1YVg0THlvH7Ew1CZ2y-ajpTts,33626
 sparseml/pytorch/sparsification/quantization/modifier_quantization.py,sha256=VQnQZozal38sffuIZjL1vKs6LeDhmiy-BvKebzewYO4,26253
 sparseml/pytorch/sparsification/quantization/quantization_scheme.py,sha256=10KNttNCHqUTNq706kPB6k7u6mvvfV0WTvx5D5Uqd-Y,12558
 sparseml/pytorch/sparsification/quantization/quantize.py,sha256=4vWbjp2WfeZ0BUf1_3BtDqLlbJfAdcrRsnzwhB5OAz8,17591
-sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=6atkPT8kxAMC_hz1r2XqQZHhjObR3wuyoL6XbHGBRZM,69959
+sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=bGDDqIeX-x6S_gjhsGr-yQOJwq8qp8D02qB5q4ZCapE,69997
 sparseml/pytorch/sparsification/training/__init__.py,sha256=4GGhQf6KVSOYwtr_WL9Xcvx4mR-k8yKMVI_zuTBHGO4,790
 sparseml/pytorch/sparsification/training/modifier_epoch.py,sha256=_5p1EZk2qbwTnWsMXbVan3vRj1IRyIM4wYYZdLGA5GE,1778
 sparseml/pytorch/sparsification/training/modifier_logging.py,sha256=K1NMqhea5EBPko6yim8CThShbiSJKN5P_ca_TCyZXto,2883
 sparseml/pytorch/sparsification/training/modifier_lr.py,sha256=m_tCydo_BHiXCHMUKZu6iqKLAP24acAT8-NLjH9RIlE,24287
 sparseml/pytorch/sparsification/training/modifier_params.py,sha256=G_0eVqu0Cup8WNLFhkfPmYnKtJlNrxcJt0FcOOdq9tA,21497
 sparseml/pytorch/sparsification/training/modifier_regularizer.py,sha256=ezHbcwI8ITgq4vwkzsWXgnq_ls6NONW_D8jEN-YR7u8,6690
 sparseml/pytorch/torchvision/__init__.py,sha256=qPAYUqRxLOdwP3JCQ79MF1N1rXaULmNQLWpqH5osPzY,744
@@ -235,15 +235,15 @@
 sparseml/pytorch/torchvision/train.py,sha256=14gq2sO3_8hKdCm3S5MPA3er7ImeLcbmi1gg3ns6sBs,41409
 sparseml/pytorch/torchvision/transforms.py,sha256=_WfLKV2G9ZLt2zdpKvaHA1ricPGufVIF-lzgKaOL2Ec,7128
 sparseml/pytorch/torchvision/utils.py,sha256=weRmF78Qf9_Kgd-L7aAHERmXKoCVqUP4J8pbSZmav58,16675
 sparseml/pytorch/utils/__init__.py,sha256=WWPrEPVj8YsCZN0JemnAF5z7hOf0nL203uixlqWoAeo,1160
 sparseml/pytorch/utils/benchmarker.py,sha256=Zw1pEj7wDe4ZU_-G0JOCymdLXydN19K1QZKzPJvBp9E,9706
 sparseml/pytorch/utils/callbacks.py,sha256=1z10T8xE0IY5mcL2ARSsHDt6sDWRVF-Nq6zVf9OvD0s,2846
 sparseml/pytorch/utils/distributed.py,sha256=lJtEvgMg6LvH9iUwhveCaWNrx_t7pjn-sOW9rfYViwI,1061
-sparseml/pytorch/utils/exporter.py,sha256=KfoPciN46ZDHKgvVk7oYBR_cyZwihRPNcCm-EvPnpfg,31056
+sparseml/pytorch/utils/exporter.py,sha256=B0HetFuxL7gDf9iTQBtkUrorPSOb58_KlAVFcUeD_mQ,31098
 sparseml/pytorch/utils/helpers.py,sha256=pCQMNjgVQN4jYuerj_6YJKGDFmOZ8-3eJMcLEw5V6-A,39284
 sparseml/pytorch/utils/log_sparsification_info.py,sha256=o9WdrrDU8W1J09NHLnW2cja5PXNq442UFzgpXf8po8M,1663
 sparseml/pytorch/utils/logger.py,sha256=KOhmFXNj46gmy5XovwQOZigBuHidVmNqDnVWMUXD7PE,31374
 sparseml/pytorch/utils/loss.py,sha256=RWFyThMBaB-7jAVuS3_CU5bmsWOVFG1jqzPciSpVsj8,27048
 sparseml/pytorch/utils/model.py,sha256=KCEZ6cNkIzLKd6N8KqJe7GX3GD-PoWErZk05nEbQuJc,11754
 sparseml/pytorch/utils/module.py,sha256=gWKNLqn8bI_q97u_QC95WkxBPAclMCwz3HmrZEHEYtU,39117
 sparseml/pytorch/utils/sparsification.py,sha256=BbH3ePC74YWGddSoLcSenLd0D_0nz-Xk5vx4Ui_KkzY,8809
@@ -309,19 +309,19 @@
 sparseml/tensorflow_v1/utils/exporter.py,sha256=RqpSP-w21SrkA_ik9WoIWdIVAAui88AiBXxRWaDZJJs,10913
 sparseml/tensorflow_v1/utils/helpers.py,sha256=40eZgnejvIki_CdupK4V1gETAgGDE9rbEXEwuNg9ASA,996
 sparseml/tensorflow_v1/utils/loss.py,sha256=4AsXh70fjp1dDcxBUzgjjpLgndwVa1CBiMG1sYi5Was,1974
 sparseml/tensorflow_v1/utils/nets_utils.py,sha256=cOTKgw7PVPEjRVU-bvcsNLdBJGTi-A7djJaUaZQwsT4,8119
 sparseml/tensorflow_v1/utils/summary.py,sha256=A2ub7KDwzsaindIuCHa7N3cRpCU6d7QbD5uNHV-R6H8,1327
 sparseml/tensorflow_v1/utils/variable.py,sha256=6ziLaNOLnxQrSPWJ2RaINqg4w-4NK9reVJWH-weK3-k,12536
 sparseml/transformers/__init__.py,sha256=0nUAFFKl3q3FUyigmXeiqvhuzCFJRZNENVwsm5j2PfY,1327
-sparseml/transformers/export.py,sha256=i5_-92O7N-t0MaNOkYSuzQ87hi9_5E3KdI0BW01R0ZM,19731
-sparseml/transformers/masked_language_modeling.py,sha256=3NVCBveaLUI-BNgTqX5Pm97-apHNFVbyNUDr5z5x1cI,30936
-sparseml/transformers/question_answering.py,sha256=koobYWD4GBcGqWkW1L005QCw4huh5rbFa8rJp_wnWko,36738
-sparseml/transformers/text_classification.py,sha256=W1e6gOcQb1vHBdhkDaJwApgFi8n3sWNmmYuKuG7WtVQ,40480
-sparseml/transformers/token_classification.py,sha256=UL1TdVCA3cZglfQNKmiJoULaEXONI4IWpDMpDrM84Q0,34530
+sparseml/transformers/export.py,sha256=Tb9UjlZAi8RqYnmRSA3GiEfzJAknpIP1nIvCVtHYPiY,20377
+sparseml/transformers/masked_language_modeling.py,sha256=xV1H7jyWCWMKTiow501cI498I5ouNC68nF7g-QNuzjw,30756
+sparseml/transformers/question_answering.py,sha256=E_Ljec9bNDrZ2KD3unTlbcRxEpyYU6C9asuEynhh4AQ,36557
+sparseml/transformers/text_classification.py,sha256=UYCpgSGTkmeGOeePQF5Idd8uY4GHQc-ShZK5SFOlP7E,40299
+sparseml/transformers/token_classification.py,sha256=6RUe1CmXQv7dHsE35aTg-xLW1g4BGakRp6pn0un2_mE,34350
 sparseml/transformers/sparsification/__init__.py,sha256=22XZNePvLFXNxp5NrcUIXzjgynCZm6jvQOErpRGlQNY,833
 sparseml/transformers/sparsification/question_answering.py,sha256=FAXhtQ8MW_2ar1dix2tQ1x1RXZuSWMLHZbVHToNWwmo,19529
 sparseml/transformers/sparsification/trainer.py,sha256=g2tP2s_W8Pmpef1CuCIsMD_teRkq9ZRIppR0Uq84Mpw,43756
 sparseml/transformers/sparsification/training_args.py,sha256=gGivIDchLi__PZMNQRmzDOaQcQLkUVFystq3LaVko3Y,1890
 sparseml/transformers/utils/__init__.py,sha256=dxyg6b2XznhBzOsduHdOalgTmoX1JC32Rb4AHns6rVk,794
 sparseml/transformers/utils/helpers.py,sha256=pgxtf0ygP7qJEVPse_dGxm7UpWSJ9JVebA_ex1c8Muw,3090
 sparseml/transformers/utils/metrics.py,sha256=ciZsxgdrzlSMnyzbgKOFE3spWsKql0z82BiYFRXiVOU,2536
@@ -349,20 +349,20 @@
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
 sparseml/yolov8/__init__.py,sha256=4akRvqiJRrRI9kcdXG3rqIiZLWIh7tvA-0zOI2zxO0w,958
 sparseml/yolov8/default.yaml,sha256=lWJc8dKEKS0PWG28pAntMe-kHym5PEXX21h9G-9zZhA,5781
 sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
 sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
-sparseml/yolov8/trainers.py,sha256=qr6iyYvyJtpTwo0Tbch-sumgMrs7ZjwG5LSBK-ywhIQ,34223
+sparseml/yolov8/trainers.py,sha256=Rj3NP6FzKo7i1ospwlh3ndOLigiQ0xqThik2s_J-VcI,34242
 sparseml/yolov8/val.py,sha256=tWKRybY-ClQ3cqf-9rMZdMwHLrSuyrSFwtqGS_8siq4,2666
 sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
 sparseml/yolov8/utils/export_samples.py,sha256=gn7et_J-OfnCTEYP0iLXx2W-HARgxqUnHqJWHBG72KM,6288
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.5.0.20230509.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.5.0.20230509.dist-info/METADATA,sha256=P4Q7V5Pbt2HCwFOkWKRy2J3CSoQwmjpanfM84ISKjbM,21295
-sparseml_nightly-1.5.0.20230509.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.5.0.20230509.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.5.0.20230509.dist-info/entry_points.txt,sha256=vz4Edi7tfmTpoq62ETf5EYJWKHltDxcPz-6GlJ8iVlI,2372
-sparseml_nightly-1.5.0.20230509.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.5.0.20230509.dist-info/RECORD,,
+sparseml_nightly-1.5.0.20230516.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.5.0.20230516.dist-info/METADATA,sha256=RvsZZZs27dyND-Xgagi3Q7ozRoFUte59YJs2oLoBh4k,21292
+sparseml_nightly-1.5.0.20230516.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.5.0.20230516.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.5.0.20230516.dist-info/entry_points.txt,sha256=vz4Edi7tfmTpoq62ETf5EYJWKHltDxcPz-6GlJ8iVlI,2372
+sparseml_nightly-1.5.0.20230516.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.5.0.20230516.dist-info/RECORD,,
```


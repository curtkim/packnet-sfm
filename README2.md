## HOWTO

    docker run --gpus all --ipc=host -v $(pwd)/checkpoints:/checkpoints -v /data:/data -it hdjang/packnet-sfm bash
    python3 scripts/infer.py --checkpoint /checkpoints/PackNet01_HR_velsup_CStoK.ckpt --input /data/datasets/KITTI_tiny/2011_09_26/2011_09_26_drive_0023_sync/image_02/data/ --output /data/datasets/packnet-sfm-output --save npz
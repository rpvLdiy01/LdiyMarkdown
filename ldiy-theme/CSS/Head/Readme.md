/**
 H1~H6的样式仓库
 **/

/* ----- ----- 2级标题的下线 ----- ----- */
#write h2::after {
    content: " ";
    position: absolute;
    bottom: 0;
    left: 0;
    position: absolute;
    height: 2px;
    width: 100%;
    background: linear-gradient(to right, rgb(136, 133, 133), rgba(148, 4, 4, 0));
}

/* ----- ----- 2级标题的序号前缀 ----- ----- */
#write h2::before {
    content: "H2";
    border-radius: .3em;
    font-size: .8em;
    padding: 3px 7px;
    margin-right: 15px;
    background-color: rgba(128, 30, 255, 1);
    color: white;
}

/* 4 5 6级标题点击后的前缀提示图标 */
/* #write>h3.md-focus:before, */
#write>h4.md-focus::before,
#write>h5.md-focus::before,
#write>h6.md-focus::before {
    width: auto;
    height: auto;
    background-color: #ff5d52;
    color: black;

    left: -1.5625rem;
    top: .375rem;
}